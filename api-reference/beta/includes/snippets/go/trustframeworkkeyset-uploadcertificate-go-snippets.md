---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29d6ba3925a9ffa3d2a7bf781b967ffbe61ec829
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088737"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
key := "key-value"
requestBody.SetKey(&key)
options := &msgraphsdk.UploadCertificateRequestBuilderPostOptions{
    Body: requestBody,
}
trustFrameworkKeySetId := "trustFrameworkKeySet-id"
result, err := graphClient.TrustFramework().KeySetsById(&trustFrameworkKeySetId).UploadCertificate().Post(options)


```