---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d244a7945a014425e7cbc56a2e9d6e601bdd97eb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322506"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationSchoolId := "educationSchool-id"
educationUserId := "educationUser-id"
graphClient.Education().SchoolsById(&educationSchoolId).UsersById(&educationUserId).Delete()


```