---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef4fe32bc493706104c8010a5face1042e3b0d8c1346dca2e1d6c599974a4a51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897802"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var following = await graphClient.Me.Drive.Following
    .Request()
    .GetAsync();

```