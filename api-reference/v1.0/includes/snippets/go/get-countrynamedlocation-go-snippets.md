---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3abb6d6871b3237357ca4f672f0c56ee9d6b792d
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287170"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

namedLocationId := "namedLocation-id"
result, err := graphClient.Identity().ConditionalAccess().NamedLocationsById(&namedLocationId).Get(nil)


```