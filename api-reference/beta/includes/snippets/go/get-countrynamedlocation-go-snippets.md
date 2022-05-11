---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87e725360831f9c616c524d96dfda5bf24f239d6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322510"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

namedLocationId := "namedLocation-id"
result, err := graphClient.Identity().ConditionalAccess().NamedLocationsById(&namedLocationId).Get()


```