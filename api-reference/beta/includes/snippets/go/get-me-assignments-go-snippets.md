---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31ecc53dfb51fa7fde9d66000c770574f3f25f08
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60998485"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Education().Me().Assignments().Get(options)


```