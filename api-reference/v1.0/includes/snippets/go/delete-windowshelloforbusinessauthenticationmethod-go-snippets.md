---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9c1ab12128ab7768b9dae56ce4db8003fa40ba9
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411286"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
windowsHelloForBusinessAuthenticationMethodId := "windowsHelloForBusinessAuthenticationMethod-id"
result, err := graphClient.UsersById(&userId).Authentication().WindowsHelloForBusinessMethodsById(&windowsHelloForBusinessAuthenticationMethodId).Delete(nil)


```