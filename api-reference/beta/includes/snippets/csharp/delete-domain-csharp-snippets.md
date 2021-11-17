---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9cb79eb35875e1d2ccd0a5d3f03a68d6cafcb0f5ce79c19a9eaacce0c886900
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102432"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Domains["{domain-id}"]
    .Request()
    .DeleteAsync();

```