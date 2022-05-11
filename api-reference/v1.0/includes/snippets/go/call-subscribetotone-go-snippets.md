---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 610dbd436d8bfee709125a3c53fc70757375c3e9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324987"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewClientContextRequestBody()
clientContext := "fd1c7836-4d84-4e24-b6aa-23188688cc54"
requestBody.SetClientContext(&clientContext)
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).SubscribeToTone(call-id).Post(requestBody)


```