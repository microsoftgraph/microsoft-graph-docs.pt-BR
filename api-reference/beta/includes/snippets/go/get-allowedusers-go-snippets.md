---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a40047731c137f295d6cb04c644d94c314f55f6a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324504"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerShareId := "printerShare-id"
result, err := graphClient.Print().SharesById(&printerShareId).AllowedUsers().Get()


```