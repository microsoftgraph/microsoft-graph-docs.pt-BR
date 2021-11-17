---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 989e7dd34fe79094e43e29604d87ece90b11a27d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019316"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

programControlId := "programControl-id"
graphClient.ProgramControlsById(&programControlId).Delete(options)


```