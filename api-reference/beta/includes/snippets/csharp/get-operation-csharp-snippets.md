---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c52f631be88ba67897ec6ecb240b4604a649de0162752253105cfbf8ef681694
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100730"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var longRunningOperation = await graphClient.Users["{user-id}"].Authentication.Operations["{longRunningOperation-id}"]
    .Request()
    .GetAsync();

```