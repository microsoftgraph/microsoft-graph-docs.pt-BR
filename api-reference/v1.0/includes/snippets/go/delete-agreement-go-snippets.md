---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b51af12a06bce7f4aba060b3abac58f843fc254d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029796"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

agreementId := "agreement-id"
graphClient.IdentityGovernance().TermsOfUse().AgreementsById(&agreementId).Delete(options)


```