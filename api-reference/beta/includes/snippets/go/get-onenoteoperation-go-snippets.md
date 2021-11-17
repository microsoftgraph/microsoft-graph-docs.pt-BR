---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe3d79a7045c42afb60fd412faad70b153b97969
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985966"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

onenoteOperationId := "onenoteOperation-id"
result, err := graphClient.Me().Onenote().OperationsById(&onenoteOperationId).Get(options)


```