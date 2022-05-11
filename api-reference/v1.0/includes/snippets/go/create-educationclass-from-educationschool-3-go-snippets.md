---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 615f720fb0268100494ce43d523b7a713b6d41da
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325641"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationSchoolId := "educationSchool-id"
educationClassId := "educationClass-id"
graphClient.Education().SchoolsById(&educationSchoolId).ClassesById(&educationClassId).Delete()


```