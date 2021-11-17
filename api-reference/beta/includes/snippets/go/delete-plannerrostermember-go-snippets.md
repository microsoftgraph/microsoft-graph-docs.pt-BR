---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 30b55d3d84ba84173a4ee884a12411a048e98885
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990034"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

plannerRosterId := "plannerRoster-id"
plannerRosterMemberId := "plannerRosterMember-id"
graphClient.Planner().RostersById(&plannerRosterId).MembersById(&plannerRosterMemberId).Delete(options)


```