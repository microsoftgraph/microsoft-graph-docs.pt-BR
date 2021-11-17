---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd09e002babbe998f09982ecba2c99f18af356a231a2894c599af6c6680dc5ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328015"
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