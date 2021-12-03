---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6bb7749cebe432ec385bb89c7f0e1c89c32071dc
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287218"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Onenote().Notebooks().Get(nil)


```