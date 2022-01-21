---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92b2b06191fceadb90a95865c8589474f073c40e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137601"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Oauth2PermissionGrants().Delta()().Get(nil)


```