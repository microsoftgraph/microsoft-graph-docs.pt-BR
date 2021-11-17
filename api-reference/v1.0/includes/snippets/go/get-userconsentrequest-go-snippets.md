---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3321a53c347b5806020415d93edd446d0dfe27a6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61008305"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

appConsentRequestId := "appConsentRequest-id"
userConsentRequestId := "userConsentRequest-id"
result, err := graphClient.IdentityGovernance().AppConsent().AppConsentRequestsById(&appConsentRequestId).UserConsentRequestsById(&userConsentRequestId).Get(options)


```