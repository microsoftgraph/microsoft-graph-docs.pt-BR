---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4f7b2ee0bd42e4974627d6a482f7bf8f5175477d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411095"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

phoneAuthenticationMethodId := "phoneAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().PhoneMethodsById(&phoneAuthenticationMethodId).Delete(nil)


```