---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd126313fdd281087661623e51e048b4b552f3b5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322297"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewItemAddress()
allowedAudiences := "me"
requestBody.SetAllowedAudiences(&allowedAudiences)
displayName := "Secret Hideout"
requestBody.SetDisplayName(&displayName)
userId := "user-id"
itemAddressId := "itemAddress-id"
graphClient.UsersById(&userId).Profile().AddressesById(&itemAddressId).Patch(requestBody)


```