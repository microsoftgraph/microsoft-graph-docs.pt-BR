---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 892162b2ecc60b9f88eaa445cd00c7795331c98a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285986"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

attributeSetId := "attributeSet-id"
result, err := graphClient.Directory().AttributeSetsById(&attributeSetId).Get(nil)


```