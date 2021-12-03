---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd54b7969480dba7dbb17ea6ab19c1fc53953368
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287034"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

namedLocationId := "namedLocation-id"
graphClient.Identity().ConditionalAccess().NamedLocationsById(&namedLocationId).Delete(nil)


```