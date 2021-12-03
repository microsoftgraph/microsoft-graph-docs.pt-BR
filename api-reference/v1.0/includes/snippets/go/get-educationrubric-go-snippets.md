---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aea6a93e2149a32e144fab463ddc82582723a007
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287260"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationRubricId := "educationRubric-id"
result, err := graphClient.Education().Me().RubricsById(&educationRubricId).Get(nil)


```