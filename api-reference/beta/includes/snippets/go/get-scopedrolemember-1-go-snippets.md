---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1610df2ed517ba57e12fca41a3612e6ceef5df19
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089903"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

administrativeUnitId := "administrativeUnit-id"
scopedRoleMembershipId := "scopedRoleMembership-id"
result, err := graphClient.AdministrativeUnitsById(&administrativeUnitId).ScopedRoleMembersById(&scopedRoleMembershipId).Get(options)


```