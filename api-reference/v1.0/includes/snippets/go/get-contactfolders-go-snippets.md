---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 557ebc97594f20cef39af75e9d91e6d29fbd3c1c
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286298"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().ContactFolders().Get(nil)


```