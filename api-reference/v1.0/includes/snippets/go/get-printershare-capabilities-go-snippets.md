---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 929a88d43113695a49c672820078f81e023a1793
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090157"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PrinterShareRequestBuilderGetQueryParameters{
    Select: "id,displayName,capabilities",
}
options := &msgraphsdk.PrinterShareRequestBuilderGetOptions{
    Q: requestParameters,
}
printerShareId := "printerShare-id"
result, err := graphClient.Print().SharesById(&printerShareId).Get(options)


```