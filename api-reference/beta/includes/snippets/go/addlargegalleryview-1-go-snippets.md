---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da30463565e1b97bab8bd3ead0b7cf17f235c719
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210435"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewClientContextRequestBody()
clientContext := "785f4929-92ca-497b-863f-c778c77c9758"
requestBody.SetClientContext(&clientContext)
options := &msgraphsdk.AddLargeGalleryViewRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).AddLargeGalleryView(call-id).Post(options)


```