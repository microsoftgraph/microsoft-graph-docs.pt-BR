---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63ce5f22a4f5cf341dc7d830da3ab97bd9c4ce95
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097447"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
graphClient.TeamsById(&teamId).Unarchive().Post(options)


```