---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91d2a340fda6f1ab56777c9749a8578b03f381a117242724ea6d82c44897705a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099465"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleDefinition = await graphClient.RoleManagement.EntitlementManagement.RoleDefinitions["{unifiedRoleDefinition-id}"]
    .Request()
    .GetAsync();

```