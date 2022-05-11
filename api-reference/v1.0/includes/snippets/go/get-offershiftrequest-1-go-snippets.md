---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4a6ae0869a170a4d90e0d771f7588a5135e423cc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324206"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
offerShiftRequestId := "offerShiftRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OfferShiftRequestsById(&offerShiftRequestId).Get()


```