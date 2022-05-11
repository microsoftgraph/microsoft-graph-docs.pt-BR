---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63c0cbb282cc4c5d3dfc214b625d31115893d116
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323195"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ContactsRequestBuilderGetQueryParameters{
    Select: "displayName,emailAddresses",
}
options := &msgraphsdk.ContactsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Me().Contacts().GetWithRequestConfigurationAndResponseHandler(options, nil)


```