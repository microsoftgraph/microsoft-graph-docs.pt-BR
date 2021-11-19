---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24fac29418af1919d6ebd52decb3fa2bf04a0b93
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087874"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

administrativeUnitId := "administrativeUnit-id"
scopedRoleMembershipId := "scopedRoleMembership-id"
graphClient.AdministrativeUnitsById(&administrativeUnitId).ScopedRoleMembersById(&scopedRoleMembershipId).Delete(options)


```