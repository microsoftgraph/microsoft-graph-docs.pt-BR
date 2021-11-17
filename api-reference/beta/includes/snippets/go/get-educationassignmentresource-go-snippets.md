---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2ebfb573b6918906821b127d7b14f681da93380
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60998596"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationAssignmentResourceId := "educationAssignmentResource-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).ResourcesById(&educationAssignmentResourceId).Get(options)


```