---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: addede8ecb890c1def2066361676e70e5526689b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396550"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationSchoolId := "educationSchool-id"
educationUserId := "educationUser-id"
graphClient.Education().SchoolsById(&educationSchoolId).UsersById(&educationUserId).Delete(nil)


```