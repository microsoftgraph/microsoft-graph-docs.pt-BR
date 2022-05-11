---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5ce818671c00f9474351cd37c2a101c8ccf63c4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324536"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationSchoolId := "educationSchool-id"
graphClient.Education().SchoolsById(&educationSchoolId).Delete()


```