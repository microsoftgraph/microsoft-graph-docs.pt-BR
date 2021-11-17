---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49381361d2fe58b7f32c8c8a69de4c0d28873cae
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026672"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

contractId := "contract-id"
result, err := graphClient.ContractsById(&contractId).Get(options)


```