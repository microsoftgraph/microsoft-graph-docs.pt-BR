---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa155577e0a6680730cc053c89ba8d6fec739c77
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324118"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlannerTask()
planId := "xqQg5FS2LkCp935s-FIFm2QAFkHM"
requestBody.SetPlanId(&planId)
bucketId := "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
requestBody.SetBucketId(&bucketId)
title := "Update client list"
requestBody.SetTitle(&title)
assignments := msgraphsdk.NewPlannerAssignments()
requestBody.SetAssignments(assignments)
assignments.SetAdditionalData(map[string]interface{}{
}
result, err := graphClient.Planner().Tasks().Post(requestBody)


```