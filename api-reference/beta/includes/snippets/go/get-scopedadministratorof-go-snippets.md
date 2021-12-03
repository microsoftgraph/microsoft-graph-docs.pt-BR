---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74cfa7f73578f18a470af813d8fce22fbbaa1930
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287324"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().ScopedRoleMemberOf().Get(nil)


```