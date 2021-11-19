---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f66d1dfdfbdce9d6776ffd15b8b2ea7cb9e891dc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101056"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
offerShiftRequestId := "offerShiftRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OfferShiftRequestsById(&offerShiftRequestId).Get(options)


```