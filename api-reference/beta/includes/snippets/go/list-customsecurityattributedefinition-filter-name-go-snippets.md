---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0ad43bb996ee6d9ac5c00c2f7031785aaa76ad13
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322816"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CustomSecurityAttributeDefinitionsRequestBuilderGetQueryParameters{
    Filter: "name%20eq%20'Project'%20and%20status%20eq%20'Available'",
}
options := &msgraphsdk.CustomSecurityAttributeDefinitionsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Directory().CustomSecurityAttributeDefinitions().GetWithRequestConfigurationAndResponseHandler(options, nil)


```