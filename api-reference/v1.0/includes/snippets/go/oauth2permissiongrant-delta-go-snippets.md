---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0139eae6b74e5e1b667ba4b06e2e99a5e97be6a9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323660"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Oauth2PermissionGrants().Delta()().Get()


```