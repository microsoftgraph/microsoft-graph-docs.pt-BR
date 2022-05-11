---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 811a5aff055048a986048fe2f030c757f2c34a38
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322446"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewKeyRequestBody()
key := "key-value"
requestBody.SetKey(&key)
trustFrameworkKeySetId := "trustFrameworkKeySet-id"
result, err := graphClient.TrustFramework().KeySetsById(&trustFrameworkKeySetId).UploadCertificate(trustFrameworkKeySet-id).Post(requestBody)


```