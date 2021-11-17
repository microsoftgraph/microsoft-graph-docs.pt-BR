---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18f871d028faf6c00c0bf1c002f401a8c98c59d1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017545"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Authentication().TemporaryAccessPassMethods().Get(options)


```