---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60fe893c688361c8bae5243795bc06045dab1305
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285873"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.IdentityGovernance().AppConsent().AppConsentRequests().Get(nil)


```