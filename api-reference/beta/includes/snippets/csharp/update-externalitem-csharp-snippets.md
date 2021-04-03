---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7803359f3c528fb426cbc91bf93cd4a6d5f5d267
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573078"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalItem = new Microsoft.Graph.ExternalConnectors.ExternalItem
{
    Acl = new List<Microsoft.Graph.ExternalConnectors.Acl>()
    {
        new Microsoft.Graph.ExternalConnectors.Acl
        {
            Type = Microsoft.Graph.ExternalConnectors.AclType.Everyone,
            Value = "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
            AccessType = Microsoft.Graph.ExternalConnectors.AccessType.Grant,
            IdentitySource = Microsoft.Graph.ExternalConnectors.IdentitySourceType.AzureActiveDirectory
        }
    }
};

await graphClient.Connections["{externalConnectors.externalConnection-id}"].Items["{externalConnectors.externalItem-id}"]
    .Request()
    .UpdateAsync(externalItem);

```