---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7239d308e315bc7c46b80d5915a51070758654b0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990069"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

plannerRosterId := "plannerRoster-id"
result, err := graphClient.Planner().RostersById(&plannerRosterId).Plans().Get(options)


```