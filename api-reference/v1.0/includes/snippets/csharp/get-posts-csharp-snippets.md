---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22862b34c114b0d7b44c78b665758ae182db8f5439189fb09c1d59297adee59d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217518"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var posts = await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"].Posts
    .Request()
    .GetAsync();

```