---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c53fe7a79c0c0554d05ab8e546522ae7af997199
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322727"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationSignInDetailedSummaryId := "applicationSignInDetailedSummary-id"
result, err := graphClient.Reports().ApplicationSignInDetailedSummaryById(&applicationSignInDetailedSummaryId).Get()


```