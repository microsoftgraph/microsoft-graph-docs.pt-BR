---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb295098f306210c8ae292f9de24f8927235f867
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016467"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

workPositionId := "workPosition-id"
graphClient.Me().Profile().PositionsById(&workPositionId).Delete(options)


```