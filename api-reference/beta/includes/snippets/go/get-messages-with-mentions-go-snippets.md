---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 615c05fc02aed976a7d07f968699aa778fd55ad1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322443"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MessagesRequestBuilderGetQueryParameters{
    Filter: "MentionsPreview/IsMentioned%20eq%20true",
    Select: "Subject,Sender,ReceivedDateTime,MentionsPreview",
}
options := &msgraphsdk.MessagesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Me().Messages().GetWithRequestConfigurationAndResponseHandler(options, nil)


```