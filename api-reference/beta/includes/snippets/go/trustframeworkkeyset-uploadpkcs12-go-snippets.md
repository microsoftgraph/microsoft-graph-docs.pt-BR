---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8c19fb4cb087959ea3ccbadd54d6631bc417466f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976941"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
key := "Base64-encoded-pfx-content"
requestBody.SetKey(&key)
password := "password-value"
requestBody.SetPassword(&password)
options := &msgraphsdk.UploadPkcs12RequestBuilderPostOptions{
    Body: requestBody,
}
trustFrameworkKeySetId := "trustFrameworkKeySet-id"
result, err := graphClient.TrustFramework().KeySetsById(&trustFrameworkKeySetId).UploadPkcs12().Post(options)


```