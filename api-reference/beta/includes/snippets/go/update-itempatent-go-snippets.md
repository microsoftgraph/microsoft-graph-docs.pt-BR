---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5eab1303087c44982a9094929446b5aa601825ce
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324273"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewItemPatent()
number := "USPTO-3954432633"
requestBody.SetNumber(&number)
webUrl := "https://patents.gov/3954432633"
requestBody.SetWebUrl(&webUrl)
userId := "user-id"
itemPatentId := "itemPatent-id"
graphClient.UsersById(&userId).Profile().PatentsById(&itemPatentId).Patch(requestBody)


```