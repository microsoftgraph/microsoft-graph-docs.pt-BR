---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91ec889371dcb6150c00749dcf714238f8533d1a7b167e38ce12c4f6332613ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101064"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"]
    .Renew()
    .Request()
    .PostAsync();

```