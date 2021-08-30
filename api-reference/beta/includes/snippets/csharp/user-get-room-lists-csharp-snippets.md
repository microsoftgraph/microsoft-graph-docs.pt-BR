---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75cf0097fbf251b34a0f69f1af61909eecea202ba4ac2dedc7582951b041a239
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160161"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var findRoomLists = await graphClient.Me
    .FindRoomLists()
    .Request()
    .GetAsync();

```