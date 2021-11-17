---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afd02c61f595d47e74500b9e74c4380afa7037abec8be6af55851bfa671b1259
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157210"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = await graphClient.Me.Messages["{message-id}"].Extensions["{extension-id}"]
    .Request()
    .GetAsync();

```