---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 492672f3e06aee104a93edddddaffde608ceae61
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285856"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
timeOffId := "timeOff-id"
graphClient.TeamsById(&teamId).Schedule().TimesOffById(&timeOffId).Delete(nil)


```