---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3516591c4e1ccaed4fed7fda10532ff936e2de15
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285956"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

agreementId := "agreement-id"
graphClient.IdentityGovernance().TermsOfUse().AgreementsById(&agreementId).Delete(nil)


```