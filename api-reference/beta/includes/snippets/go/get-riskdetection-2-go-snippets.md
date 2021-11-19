---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c350f5d6a6c265d1468dd8894c7f6d966126479e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090884"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

riskDetectionId := "riskDetection-id"
result, err := graphClient.IdentityProtection().RiskDetectionsById(&riskDetectionId).Get(options)


```