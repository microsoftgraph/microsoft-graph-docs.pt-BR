---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d887f9756a01acf8e4b48284df2ba357496268177e67dae600ed0b2df7299a9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275014"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var services = await graphClient.Print.Services
    .Request()
    .GetAsync();

```