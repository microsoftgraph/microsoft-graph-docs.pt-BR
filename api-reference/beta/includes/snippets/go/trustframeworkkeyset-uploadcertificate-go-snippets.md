---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a474619e8e0a6a82a4c15427ee91e7753a80f377
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411201"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewKeyRequestBody()
key := "key-value"
requestBody.SetKey(&key)
options := &msgraphsdk.UploadCertificateRequestBuilderPostOptions{
    Body: requestBody,
}
trustFrameworkKeySetId := "trustFrameworkKeySet-id"
result, err := graphClient.TrustFramework().KeySetsById(&trustFrameworkKeySetId).UploadCertificate(trustFrameworkKeySet-id).Post(options)


```