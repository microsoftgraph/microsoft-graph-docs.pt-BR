---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8e78fb10398e2138b927e9d3d44d86625ce6b56
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092862"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeCards().Post(options)


```