---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1e41798fbd2fec018474eb9e9c2838820bec742
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090306"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Profile().Positions().Get(options)


```