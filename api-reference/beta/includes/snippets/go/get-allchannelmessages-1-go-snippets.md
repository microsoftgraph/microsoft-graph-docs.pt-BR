---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b60adcbdfed44ce2626f9e401b4c606a804ffe1d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323634"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().GetAllMessages()(team-id).Get()


```