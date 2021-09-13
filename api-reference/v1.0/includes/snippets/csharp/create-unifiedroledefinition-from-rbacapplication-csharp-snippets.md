---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77fafb086743f0064111174b725e4a27c5dee0fc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59110488"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleDefinition = new UnifiedRoleDefinition
{
    Description = "Update basic properties of application registrations",
    DisplayName = "Application Registration Support Administrator",
    RolePermissions = new List<UnifiedRolePermission>()
    {
        new UnifiedRolePermission
        {
            AllowedResourceActions = new List<String>()
            {
                "microsoft.directory/applications/basic/read"
            }
        }
    },
    IsEnabled = true
};

await graphClient.RoleManagement.Directory.RoleDefinitions
    .Request()
    .AddAsync(unifiedRoleDefinition);

```