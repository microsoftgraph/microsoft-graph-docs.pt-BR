---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df26463b1843d6e30b47ec0972bf4167162de498
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324250"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
use := "use-value"
requestBody.SetUse(&use)
k := "application-secret-to-be-uploaded"
requestBody.SetK(&k)
nbf := int64(1508969811)
requestBody.SetNbf(&nbf)
exp := int64(1508973711)
requestBody.SetExp(&exp)
trustFrameworkKeySetId := "trustFrameworkKeySet-id"
result, err := graphClient.TrustFramework().KeySetsById(&trustFrameworkKeySetId).UploadSecret(trustFrameworkKeySet-id).Post(requestBody)


```