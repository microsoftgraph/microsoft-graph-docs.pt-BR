---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4c4fc9a801cc9632fd1e5437696ef64f499867fe
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216977"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shares = await graphClient.Print.Shares
    .Request()
    .GetAsync();

```