---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 630bb6c5df73d85c0b7ef64f83612cf89518b692
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440860"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mobileAppManagementPolicies = await graphClient.Policies.MobileAppManagementPolicies
    .Request()
    .GetAsync();

```