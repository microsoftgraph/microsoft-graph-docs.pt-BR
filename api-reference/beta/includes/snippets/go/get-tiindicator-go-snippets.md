---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de4486a79dfcb4f4b7fdb864a3d11c7ccf77c69e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097435"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tiIndicatorId := "tiIndicator-id"
result, err := graphClient.Security().TiIndicatorsById(&tiIndicatorId).Get(options)


```