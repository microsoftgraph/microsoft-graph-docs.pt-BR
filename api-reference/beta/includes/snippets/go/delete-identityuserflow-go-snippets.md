---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe10a8defe43a89ea52bd551054d229f23525971
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087436"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityUserFlowId := "identityUserFlow-id"
graphClient.Identity().UserFlowsById(&identityUserFlowId).Delete(options)


```