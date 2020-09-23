---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 093a33ea1b94acb56e7bd07aacda75bdbbb9ced0
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223050"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.External.Connections["contosohr"].Groups["31bea3d537902000"]
    .Request()
    .DeleteAsync();

```