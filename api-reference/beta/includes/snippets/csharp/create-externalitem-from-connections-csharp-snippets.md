---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5dc48df8356f20c9aa02b70914a41ac69a6c43ff
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683985"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalItem = new ExternalItem
{
    Acl = new List<Acl>()
    {
        new Acl
        {
            Type = AclType.User,
            Value = "49103559-feac-4575-8b94-254814dfca72",
            AccessType = AccessType.Deny,
            IdentitySource = "Azure Active Directory"
        }
    },
    Properties = new Properties
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"title", "Error in the payment gateway"},
            {"priority", "1"},
            {"assignee", "john@contoso.com"}
        }
    },
    Content = new ExternalItemContent
    {
        Value = "<h1>Error in payment gateway</h1><p>Error details...</p>",
        Type = ExternalItemContentType.Html
    }
};

await graphClient.Connections["contosohr"].Items["TSP228082938"]
    .Request()
    .PutAsync(externalItem);

```