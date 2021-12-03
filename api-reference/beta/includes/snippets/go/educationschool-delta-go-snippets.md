---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 180d058b26a037a4976b44b204c5967485aa5002
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285866"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationSchoolId := "educationSchool-id"
result, err := graphClient.Education().SchoolsById(&educationSchoolId).Get(nil)


```