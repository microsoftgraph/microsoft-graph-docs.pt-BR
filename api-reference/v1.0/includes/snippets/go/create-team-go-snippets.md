---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9e4c03285b76f2c5e80368bfcfcb980960f65a4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325088"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
}
groupId := "group-id"
graphClient.GroupsById(&groupId).Team().Put(requestBody)


```