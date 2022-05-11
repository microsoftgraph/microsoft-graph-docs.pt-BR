---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dec5ea4bd37a48105da8e5f5e99fdfb89a3ed045
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325098"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

placeId := "place-id"
result, err := graphClient.PlacesById(&placeId).Get()


```