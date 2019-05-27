---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72a55c21f4a58e4a1affc4bfcec6f8faa01f0287
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455081"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Drive.Root.Delta()
    .Request()
    .GetAsync();

```