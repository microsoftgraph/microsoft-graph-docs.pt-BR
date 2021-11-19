---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62ad1b422fc12f6922a16020e4cea6cc7a5a530e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089249"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerId := "printer-id"
printTaskTriggerId := "printTaskTrigger-id"
result, err := graphClient.Print().PrintersById(&printerId).TaskTriggersById(&printTaskTriggerId).Get(options)


```