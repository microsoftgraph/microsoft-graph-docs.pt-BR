---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7f1370d023dc9ec9fb135f3ca98c2a89552cf650
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286951"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityUserFlowAttributeId := "identityUserFlowAttribute-id"
result, err := graphClient.Identity().UserFlowAttributesById(&identityUserFlowAttributeId).Get(nil)


```