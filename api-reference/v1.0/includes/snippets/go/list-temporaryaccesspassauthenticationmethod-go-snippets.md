---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1b6975561fe5fc71d8baa9d9382614bd727bfc0
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093403"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).Authentication().TemporaryAccessPassMethods().Get()


```