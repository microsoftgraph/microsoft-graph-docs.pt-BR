---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dcb4b0d4b76cd6a5cf643301e012c7389da1d49e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083151"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerRosterId := "plannerRoster-id"
graphClient.Planner().RostersById(&plannerRosterId).Delete(options)


```