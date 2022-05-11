---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94654fa44362c7fcbc53eb1322d2bbff0f0213d1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325274"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personAnnotationId := "personAnnotation-id"
result, err := graphClient.Me().Profile().NotesById(&personAnnotationId).Get()


```