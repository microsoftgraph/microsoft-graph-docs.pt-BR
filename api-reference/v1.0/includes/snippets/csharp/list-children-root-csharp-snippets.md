---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a459da7a60b66fba94f15f9ec54926fe710af0ea296e216b297c5411f9269d1e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899337"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Root.Children
    .Request()
    .GetAsync();

```