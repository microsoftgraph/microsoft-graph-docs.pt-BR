---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7677296903ddba4ec7fba7a8c981451645a09398
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025098"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printerId := "printer-id"
graphClient.Print().PrintersById(&printerId).RestoreFactoryDefaults().Post(options)


```