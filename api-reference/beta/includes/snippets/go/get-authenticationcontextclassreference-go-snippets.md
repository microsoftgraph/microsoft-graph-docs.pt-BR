---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13026c10ee979c8e8c81201b8daa2705477d4814
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096173"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Identity().ConditionalAccess().AuthenticationContextClassReferences().Get(options)


```