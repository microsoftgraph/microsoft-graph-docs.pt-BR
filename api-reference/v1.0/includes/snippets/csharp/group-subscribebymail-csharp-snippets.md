---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca1e924cded9187375c9b27d53d946543b56f9a02b077ea875d615081d823899
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329711"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"]
    .SubscribeByMail()
    .Request()
    .PostAsync();

```