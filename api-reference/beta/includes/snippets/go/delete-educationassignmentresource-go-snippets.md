---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: efeb82b0699a8c79854cb78c1180c39b5944e24e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324280"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationAssignmentResourceId := "educationAssignmentResource-id"
graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).ResourcesById(&educationAssignmentResourceId).Delete()


```