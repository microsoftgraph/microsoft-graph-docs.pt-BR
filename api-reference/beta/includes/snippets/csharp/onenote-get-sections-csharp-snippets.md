---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 384747d711f0a99f39e33fa69b7832e3dcdb0570a6f82d9564b4eb2cbdf4f5ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327653"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sections = await graphClient.Me.Onenote.Sections
    .Request()
    .GetAsync();

```