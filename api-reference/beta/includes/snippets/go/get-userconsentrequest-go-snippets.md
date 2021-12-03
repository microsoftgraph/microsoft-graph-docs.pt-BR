---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f7cee968e38f46c8d742647760ee4f89a053a57
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285989"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

appConsentRequestId := "appConsentRequest-id"
userConsentRequestId := "userConsentRequest-id"
result, err := graphClient.IdentityGovernance().AppConsent().AppConsentRequestsById(&appConsentRequestId).UserConsentRequestsById(&userConsentRequestId).Get(nil)


```