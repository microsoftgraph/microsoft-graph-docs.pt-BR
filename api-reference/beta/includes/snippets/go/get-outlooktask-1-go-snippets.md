---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8b1f083c5e73cf0dddd6e34fce21f08b73e6bc42
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287311"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

outlookTaskId := "outlookTask-id"
result, err := graphClient.Me().Outlook().TasksById(&outlookTaskId).Get(nil)


```