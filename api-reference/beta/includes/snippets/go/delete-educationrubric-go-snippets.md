---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aafa7a1999533490865700c1a559853aec204547
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324418"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationRubricId := "educationRubric-id"
graphClient.Education().Me().RubricsById(&educationRubricId).Delete()


```