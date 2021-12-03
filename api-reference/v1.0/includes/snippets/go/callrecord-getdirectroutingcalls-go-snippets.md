---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2103844216485043fa6d3767f39ff457fa1654be
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286726"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callRecordId := "callRecord-id"
result, err := graphClient.Communications().CallRecordsById(&callRecordId).Get(nil)


```