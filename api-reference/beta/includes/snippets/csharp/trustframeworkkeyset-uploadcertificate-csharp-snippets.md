---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4771bd5b1bba88c10fcc7a7b274e8ba934dfd71a8e14b1ca82f0257b60ef150
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099590"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var key = "key-value";

await graphClient.TrustFramework.KeySets["{trustFrameworkKeySet-id}"]
    .UploadCertificate(key)
    .Request()
    .PostAsync();

```