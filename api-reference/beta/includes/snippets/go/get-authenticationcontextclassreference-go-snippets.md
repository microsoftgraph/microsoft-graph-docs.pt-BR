---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf67ab44d86901f7fe86f070c4dfa8895f3595d3
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629792"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Identity().ConditionalAccess().AuthenticationContextClassReferences().Get()


```