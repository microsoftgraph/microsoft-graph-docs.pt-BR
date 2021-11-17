---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9c541757e2ed4fa6f1c55e6b6f64aac6f09539f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033365"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().OwnedObjects().Get(options)


```