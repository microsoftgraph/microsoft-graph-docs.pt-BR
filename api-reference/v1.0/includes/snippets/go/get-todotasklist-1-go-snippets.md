---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 011cb7211707dd02c07beba300a68a2696205977
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60973540"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Todo().Lists().Get(options)


```