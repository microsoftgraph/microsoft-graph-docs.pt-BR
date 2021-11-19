---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7d40503629f187b346eb41be33dce09d5bd3f42e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101802"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Outlook().TaskGroups().Get(options)


```