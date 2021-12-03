---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8d46d6a98a8f93aa83a5d09e5f785684ac7fc7a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287263"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationAssignmentResourceId := "educationAssignmentResource-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).ResourcesById(&educationAssignmentResourceId).Get(nil)


```