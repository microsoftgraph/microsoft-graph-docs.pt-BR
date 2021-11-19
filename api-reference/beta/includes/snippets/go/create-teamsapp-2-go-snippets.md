---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4b4e412bc8899629fb892bf939b421e0ebc7702a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091805"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TeamsAppsRequestBuilderPostQueryParameters{
    RequiresReview: true,
}
options := &msgraphsdk.TeamsAppsRequestBuilderPostOptions{
    Q: requestParameters,
}
graphClient.AppCatalogs().TeamsApps().Post(options)


```