---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e036c4b9fdd593d88f4163b30b57ab23076af65604b40affc3d46355e381fd10
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101994"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Columns
    .Request()
    .GetAsync();

```