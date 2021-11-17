---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5412fb0592610dc5dc90ce6072c520745f32977
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996866"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Settings().RegionalAndLanguageSettings().Get(options)


```