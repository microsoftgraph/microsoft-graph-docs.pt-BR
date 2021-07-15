---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2fafc549f8b8bd3761596cd15e11ade506577456
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442228"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleDefinitions = await graphClient.RoleManagement.EntitlementManagement.RoleDefinitions
    .Request()
    .GetAsync();

```