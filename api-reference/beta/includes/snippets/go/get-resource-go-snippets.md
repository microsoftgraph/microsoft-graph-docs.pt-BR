---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: deaca4ddb7a79c39c55575cf8265d47f9bcacc3d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325436"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onenoteResourceId := "onenoteResource-id"
graphClient.Me().Onenote().ResourcesById(&onenoteResourceId).Content().Get()


```