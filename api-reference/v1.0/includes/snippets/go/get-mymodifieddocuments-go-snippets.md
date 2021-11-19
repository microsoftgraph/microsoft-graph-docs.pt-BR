---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f293c953705cd6d12390a5cc8b22d1b2e7295362
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089003"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Insights().Used().Get(options)


```