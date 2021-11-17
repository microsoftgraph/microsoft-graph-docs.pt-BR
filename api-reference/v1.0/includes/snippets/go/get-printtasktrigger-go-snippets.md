---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 299c9c3e13dbe925214ff8707d7ca0e5693f63ed
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025042"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printerId := "printer-id"
printTaskTriggerId := "printTaskTrigger-id"
result, err := graphClient.Print().PrintersById(&printerId).TaskTriggersById(&printTaskTriggerId).Get(options)


```