---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5fcec3dd7ae7e2a5217cb2113014a4b2c41da05
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082130"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerId := "printer-id"
printTaskTriggerId := "printTaskTrigger-id"
graphClient.Print().PrintersById(&printerId).TaskTriggersById(&printTaskTriggerId).Delete(options)


```