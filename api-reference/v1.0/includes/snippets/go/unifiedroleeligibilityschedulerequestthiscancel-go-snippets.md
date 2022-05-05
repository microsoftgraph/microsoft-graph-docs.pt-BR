---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72d97b6883fc8586a78fa59296b361848cc99bfe
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204785"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleEligibilityScheduleRequestId := "unifiedRoleEligibilityScheduleRequest-id"
graphClient.RoleManagement().Directory().RoleEligibilityScheduleRequestsById(&unifiedRoleEligibilityScheduleRequestId).Cancel(unifiedRoleEligibilityScheduleRequest-id).Post(nil)


```