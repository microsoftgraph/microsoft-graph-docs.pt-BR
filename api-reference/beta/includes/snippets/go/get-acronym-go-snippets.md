---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55e3f812ea6b5d03048f8755fd687286d7588c05
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324053"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

acronymId := "acronym-id"
result, err := graphClient.Search().AcronymsById(&acronymId).Get()


```