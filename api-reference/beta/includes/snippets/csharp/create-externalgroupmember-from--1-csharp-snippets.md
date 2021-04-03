---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70e8f99331079e6057fff3ee77738119a7f5c3ec
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573075"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroupMember = new ExternalGroupMember
{
    Id = "e811976d-83df-4cbd-8b9b-5215b18aa874",
    Type = Microsoft.Graph.ExternalConnectors.ExternalGroupMemberType.User,
    IdentitySource = Microsoft.Graph.ExternalConnectors.IdentitySourceType.AzureActiveDirectory
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"].Members
    .Request()
    .AddAsync(externalGroupMember);

```