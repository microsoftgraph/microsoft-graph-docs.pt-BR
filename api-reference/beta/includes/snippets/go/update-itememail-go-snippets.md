---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa63e6d9cae206ae93e555b68011970af1450c9f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324839"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewItemEmail()
displayName := "Business Email"
requestBody.SetDisplayName(&displayName)
type := "work"
requestBody.SetType(&type)
userId := "user-id"
itemEmailId := "itemEmail-id"
graphClient.UsersById(&userId).Profile().EmailsById(&itemEmailId).Patch(requestBody)


```