---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2534e702796c2707f5ba04c88bea3602fe3f0f308a13aa7df23c7b00c6e24ad4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102475"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].Permissions["{permission-id}"]
    .Request()
    .DeleteAsync();

```