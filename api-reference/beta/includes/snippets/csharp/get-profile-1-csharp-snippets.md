---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8625372d247ad5bc20bf31f04871798438b75f25a30839670d7ce0d1d33f7b7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272096"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profile = await graphClient.Me.Profile
    .Request()
    .GetAsync();

```