---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b567e53b5768761fed8b01a30d998804722f0fbb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081681"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

namedLocationId := "namedLocation-id"
result, err := graphClient.Identity().ConditionalAccess().NamedLocationsById(&namedLocationId).Get(options)


```