---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa9b322aed2a9fce9964386070d845366c31b4fb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089460"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityUserFlowId := "identityUserFlow-id"
result, err := graphClient.Identity().UserFlowsById(&identityUserFlowId).Get(options)


```