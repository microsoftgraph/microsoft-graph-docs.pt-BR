---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2a509ff581d302e3c6d7570a0c9c9ebf59e7d7b3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086792"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerId := "printer-id"
result, err := graphClient.Print().PrintersById(&printerId).Connectors().Get(options)


```