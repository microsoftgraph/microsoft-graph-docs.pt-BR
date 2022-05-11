---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd240a0de8b210ab9e125eb46d5d511bcb007b2a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322433"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationRubric()
displayName := "Example Credit Rubric after display name patch"
requestBody.SetDisplayName(&displayName)
educationRubricId := "educationRubric-id"
graphClient.Education().Me().RubricsById(&educationRubricId).Patch(requestBody)


```