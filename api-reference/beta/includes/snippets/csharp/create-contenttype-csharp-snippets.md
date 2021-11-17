---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbd9eac394ca1a770b2ac0f83ccc95b6e1c025a3304c837918b940ed959f42ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214067"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentType = new ContentType
{
    Name = "docSet",
    Description = "custom docset",
    Base = new ContentType
    {
        Name = "Document Set",
        Id = "0x0120D520"
    },
    Group = "Document Set Content Types"
};

await graphClient.Sites["{site-id}"].ContentTypes
    .Request()
    .AddAsync(contentType);

```