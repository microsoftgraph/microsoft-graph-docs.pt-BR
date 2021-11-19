---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08a10c96ce11364675309635ce9082896233c5eb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092206"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Members().Get(options)


```