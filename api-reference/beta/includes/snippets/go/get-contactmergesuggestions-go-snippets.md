---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99905a07f18fbe6bf3ad5023a4902c183a9fc286
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393960"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Settings().ContactMergeSuggestions().Get(nil)


```