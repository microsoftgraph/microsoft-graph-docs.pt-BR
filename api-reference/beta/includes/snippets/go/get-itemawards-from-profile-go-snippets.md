---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6e0bc32ff77fee2453f32d8cded4ccc2ea6dcdf
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019526"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Profile().Awards().Get(options)


```