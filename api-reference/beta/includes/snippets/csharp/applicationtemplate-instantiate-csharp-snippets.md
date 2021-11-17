---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f461727d8a9ca43ac4473e6243fc7974e08823ea2931ea5a2edb048117079289
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100580"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "My custom name";

await graphClient.ApplicationTemplates["{applicationTemplate-id}"]
    .Instantiate(displayName)
    .Request()
    .PostAsync();

```