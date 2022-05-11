---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9cab79bdf142c1749d2b881928a8efc4594dfbd3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322969"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

appConsentRequestId := "appConsentRequest-id"
result, err := graphClient.IdentityGovernance().AppConsent().AppConsentRequestsById(&appConsentRequestId).UserConsentRequests().Get()


```