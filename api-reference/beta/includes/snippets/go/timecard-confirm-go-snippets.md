---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfcecb6831829ec045960a991e3fe827102492bf
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286843"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
timeCardId := "timeCard-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeCardsById(&timeCardId).Confirm().Post(nil)


```