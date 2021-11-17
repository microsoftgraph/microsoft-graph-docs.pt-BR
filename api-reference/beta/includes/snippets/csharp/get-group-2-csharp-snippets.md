---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c36595f2193a31330e029aa1410b1da8e6dd91e1b5dcf31ef82bba29aa965c9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157592"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.TermStore.Groups
    .Request()
    .GetAsync();

```