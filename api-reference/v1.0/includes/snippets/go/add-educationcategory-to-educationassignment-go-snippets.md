---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea6556e3979cad8648cff2f6539d23f7beafffd2
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946741"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationCategoryId := "educationCategory-id"
graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).CategoriesById(&educationCategoryId).$ref().Delete()


```