---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c90708a40eb030941fe0fee56ccdf7a2ca1ab576ae087432070f8a9d13342b26
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273210"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var store = await graphClient.Sites["{site-id}"].TermStore
    .Request()
    .GetAsync();

```