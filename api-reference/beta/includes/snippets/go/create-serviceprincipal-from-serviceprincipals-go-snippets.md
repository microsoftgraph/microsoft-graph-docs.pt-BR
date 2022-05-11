---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 603a21db65a47313d891321f30b7f918172f6941
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325266"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewServicePrincipal()
appId := "65415bb1-9267-4313-bbf5-ae259732ee12"
requestBody.SetAppId(&appId)
result, err := graphClient.ServicePrincipals().Post(requestBody)


```