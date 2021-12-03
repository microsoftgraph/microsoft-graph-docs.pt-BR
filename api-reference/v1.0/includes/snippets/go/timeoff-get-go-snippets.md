---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 076c7c1767ff42ada36cff487e2c814d1f47c8ff
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286430"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
timeOffId := "timeOff-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimesOffById(&timeOffId).Get(nil)


```