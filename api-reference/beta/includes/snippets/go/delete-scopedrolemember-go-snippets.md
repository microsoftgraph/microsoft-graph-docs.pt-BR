---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58557099295d8fc9b76ad7e127d23fb1fef36a9c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410948"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

administrativeUnitId := "administrativeUnit-id"
scopedRoleMembershipId := "scopedRoleMembership-id"
result, err := graphClient.AdministrativeUnitsById(&administrativeUnitId).ScopedRoleMembersById(&scopedRoleMembershipId).Delete(nil)


```