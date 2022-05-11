---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc58c708507fb7b8251e01fd925a1acb20dd78f7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323745"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewInferenceClassificationOverride()
classifyAs := "focused"
requestBody.SetClassifyAs(&classifyAs)
senderEmailAddress := msgraphsdk.NewEmailAddress()
requestBody.SetSenderEmailAddress(senderEmailAddress)
name := "Samantha Booth"
senderEmailAddress.SetName(&name)
address := "samanthab@adatum.onmicrosoft.com"
senderEmailAddress.SetAddress(&address)
result, err := graphClient.Me().InferenceClassification().Overrides().Post(requestBody)


```