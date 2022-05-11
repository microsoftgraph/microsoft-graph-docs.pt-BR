---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 579be912b8101a36a395c168b09d3c5b59c98696
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325366"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerRosterId := "plannerRoster-id"
plannerRosterMemberId := "plannerRosterMember-id"
graphClient.Planner().RostersById(&plannerRosterId).MembersById(&plannerRosterMemberId).Delete()


```