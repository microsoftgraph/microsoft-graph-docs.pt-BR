---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 985e9e057bd8ada3a3805b89034ba377a845e955
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433369"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var windowsHelloForBusinessMethods = await graphClient.Users["annie@contoso.com"].Authentication.WindowsHelloForBusinessMethods
    .Request()
    .GetAsync();

```