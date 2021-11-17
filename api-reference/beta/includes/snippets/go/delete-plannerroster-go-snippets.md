---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c096d16c03eeb7ef0c06b275529eeacdc8f024d9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019701"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

plannerRosterId := "plannerRoster-id"
graphClient.Planner().RostersById(&plannerRosterId).Delete(options)


```