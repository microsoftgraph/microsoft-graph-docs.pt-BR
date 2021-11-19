---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd6198dbcc9a49c2383d363ab51d2fb265c2eb42
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096000"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().CalendarGroups().Get(options)


```