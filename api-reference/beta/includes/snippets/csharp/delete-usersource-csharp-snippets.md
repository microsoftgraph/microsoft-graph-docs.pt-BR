---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa4e6c6dd22b42bbc82672a6803475736f404baa
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657198"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["4c8f8f70-7785-4bd4-b296-c98376a2c5e1"].Custodians["2192ca408ea2410eba3bec8ae873be6b"].UserSources["46384443-4137-3032-3437-363939433735"]
    .Request()
    .DeleteAsync();

```