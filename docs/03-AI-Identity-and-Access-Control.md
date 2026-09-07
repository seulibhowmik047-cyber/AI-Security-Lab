
---

# 4️⃣ `docs/03-AI-Identity-and-Access-Control.md`

```markdown
# AI Identity and Access Control

## Authentication

Authentication answers:

> Who are you?

Examples:

- User authentication
- Application authentication
- Managed Identity

---

## Authorization

Authorization answers:

> What are you allowed to do?

Authorization determines which resources and actions an identity can access.

---

## Least Privilege

AI applications and agents should receive only the permissions required to perform their intended tasks.

### Example

A document-analysis agent should only have access to resources required for document analysis.

It should not automatically receive access to:

- Payroll
- HR data
- Finance systems
- Unrelated SharePoint resources

---

## Managed Identity

Managed Identity allows Azure resources to authenticate to supported Azure services without storing credentials directly in application code.

---

## RBAC

Role-Based Access Control can be used to control what an identity can do on Azure resources.

---

## Security Flow

```text
AI Application
      |
      v
Managed Identity
      |
      v
Microsoft Entra ID
      |
      v
RBAC Authorization
      |
      v
Azure Resource
