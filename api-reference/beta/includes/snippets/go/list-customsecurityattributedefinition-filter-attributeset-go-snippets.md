---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a7d47a8719b8b242e22ff8b695e16bcb84db49ea
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322817"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CustomSecurityAttributeDefinitionsRequestBuilderGetQueryParameters{
    Filter: "attributeSet%20eq%20'Engineering'%20and%20status%20eq%20'Available'%20and%20type%20eq%20'String'",
}
options := &msgraphsdk.CustomSecurityAttributeDefinitionsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Directory().CustomSecurityAttributeDefinitions().GetWithRequestConfigurationAndResponseHandler(options, nil)


```