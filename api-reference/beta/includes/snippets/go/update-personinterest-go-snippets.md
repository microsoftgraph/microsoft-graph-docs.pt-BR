---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9b4c846fb9304027d0efb458b31d56fb8ea84756
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323108"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonInterest()
requestBody.SetCategories( []String {
    "Sports",
}
personInterestId := "personInterest-id"
graphClient.Me().Profile().InterestsById(&personInterestId).Patch(requestBody)


```