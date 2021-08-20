---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc8fd481ac375078d8755dede5db577f5c36b63c
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368798"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mobileDeviceManagementPolicies = await graphClient.Policies.MobileDeviceManagementPolicies
    .Request()
    .GetAsync();

```