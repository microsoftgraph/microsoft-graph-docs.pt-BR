---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 622a3cecd86662f4dab0286cafdd508fe2369f37
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324309"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).TransitiveMemberOf().Get()


```