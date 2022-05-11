---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 298a9417848908e8f00623c877e32ba61d23a2b9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324381"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
timeOffId := "timeOff-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimesOffById(&timeOffId).Get()


```