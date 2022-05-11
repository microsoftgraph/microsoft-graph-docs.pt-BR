---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25768ec9166d06a55b0e5a291a83a5d01a1261b2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324265"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerId := "printer-id"
graphClient.Print().PrintersById(&printerId).RestoreFactoryDefaults(printer-id).Post()


```