---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb26f0b0521881c005e153ec49283916421312b8e37074dc09898cfc10b7ff9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217105"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var verifiedPublisherId = "1234567";

await graphClient.Applications["{application-id}"]
    .SetVerifiedPublisher(verifiedPublisherId)
    .Request()
    .PostAsync();

```