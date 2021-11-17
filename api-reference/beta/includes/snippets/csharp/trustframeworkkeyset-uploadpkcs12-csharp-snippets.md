---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3543aa71fb7e212fb84bdda750e7d3adbf087a258f3fdb6ba8088c57de40d3fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326940"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var key = "Base64-encoded-pfx-content";

var password = "password-value";

await graphClient.TrustFramework.KeySets["{trustFrameworkKeySet-id}"]
    .UploadPkcs12(key,password)
    .Request()
    .PostAsync();

```