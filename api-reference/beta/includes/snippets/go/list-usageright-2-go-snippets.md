---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb22e5f2efc31cde4aea8f9acee1a1ffbfbefce4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098029"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsageRightsRequestBuilderGetQueryParameters{
    Filter: "state%20in%20('active',%20'suspended')%20and%20serviceIdentifier%20in%20('ABCD')",
}
options := &msgraphsdk.UsageRightsRequestBuilderGetOptions{
    Q: requestParameters,
}
deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).UsageRights().Get(options)


```