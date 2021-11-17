---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b60001e313740b341f1e33c51795e00e85f0cae783042ea51000a64a59fec8a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102826"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeCard = await graphClient.Teams["{team-id}"].Schedule.TimeCards["{timeCard-id}"]
    .Request()
    .GetAsync();

```