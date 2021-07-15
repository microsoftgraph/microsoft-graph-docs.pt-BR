---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8dacedb03d0ea22043f318a1798639ecf04565a6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440699"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleDefinition = await graphClient.RoleManagement.EntitlementManagement.RoleDefinitions["{unifiedRoleDefinition-id}"]
    .Request()
    .GetAsync();

```