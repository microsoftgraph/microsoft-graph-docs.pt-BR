---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56e1199df815ade3b40195d14028f0586ff042a29a952cf02775299a3be027fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159080"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

using var stream = new System.IO.MemoryStream(Encoding.UTF8.GetBytes(@"Binary data for the image"));

await graphClient.Me.Photo.Content
    .Request()
    .PutAsync(stream);

```