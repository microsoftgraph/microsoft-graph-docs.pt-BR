---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5730c252ff19a50208a54905fd8c05c9ea4f607
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027961"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Profile().WebAccounts().Get(options)


```