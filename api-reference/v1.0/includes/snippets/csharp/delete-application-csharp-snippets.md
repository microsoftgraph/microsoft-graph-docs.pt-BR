---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1cec813d33e900e5a61d5a4c804a7334f367f6e29cbddc2e98580cde29aa9b3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275372"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{application-id}"]
    .Request()
    .DeleteAsync();

```