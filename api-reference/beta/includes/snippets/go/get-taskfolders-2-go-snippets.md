---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 172561c3d1c223b62856893fd345296b1384068d
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286971"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Outlook().TaskFolders().Get(nil)


```