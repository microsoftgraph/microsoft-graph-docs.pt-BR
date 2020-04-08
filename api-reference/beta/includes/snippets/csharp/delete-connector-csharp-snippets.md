---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1a9477e3294d73efea7db7a12cbb0023db181d8
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "42948168"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Connectors["{id}"]
    .Request()
    .DeleteAsync();

```