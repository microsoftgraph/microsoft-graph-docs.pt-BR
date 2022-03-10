---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72845aad3d99b0f1fc53b8b25ebcab7abeae0fff
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410895"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
itemPhoneId := "itemPhone-id"
result, err := graphClient.UsersById(&userId).Profile().PhonesById(&itemPhoneId).Delete(nil)


```