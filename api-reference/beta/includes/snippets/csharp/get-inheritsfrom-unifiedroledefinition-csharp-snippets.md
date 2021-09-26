---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 460a3ac3e8ec4658904dbf216fd060d843ed0e886cc71eb74a73adafdd35a604
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099466"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleDefinition = await graphClient.RoleManagement.Directory.RoleDefinitions["{unifiedRoleDefinition-id}"]
    .Request()
    .Expand("inheritsPermissionsFrom")
    .GetAsync();

```