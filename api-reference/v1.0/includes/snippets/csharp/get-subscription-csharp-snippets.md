---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be28631bbbb29dcec26ed0d05f984950f39b59f55aede637b1726d50c050c440
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102390"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = await graphClient.Subscriptions["{subscription-id}"]
    .Request()
    .GetAsync();

```