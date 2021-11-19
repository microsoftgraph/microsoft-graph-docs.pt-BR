---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a231a8edf9c9ffe7fd34599890b2faf3c2ab81df
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102230"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Contacts().Get(options)


```