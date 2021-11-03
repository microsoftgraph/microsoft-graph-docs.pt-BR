---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 793f3efc4c9e4f7a3799816a6044e6447fa1533e4d43e3bfda4b180031bf093c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274967"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"]
    .Publish()
    .Request()
    .PostAsync();

```