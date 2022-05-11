---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3671cfa038c88384351c174a4b791f44e7d17563
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325047"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
contentSharingSessionId := "contentSharingSession-id"
result, err := graphClient.Communications().CallsById(&callId).ContentSharingSessionsById(&contentSharingSessionId).Get()


```