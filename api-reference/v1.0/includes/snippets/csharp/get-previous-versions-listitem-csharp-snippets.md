---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a67bcb91dddf3be24cda0fb42f166e384637a66f63211ad6962c0ee493811907
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275313"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var versions = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"].Versions
    .Request()
    .GetAsync();

```