---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: feea92b09324297e1b7ee36e1379205eb0ec825920768568cfaee565f3cfa473
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216668"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sites = await graphClient.Sites
    .Request()
    .Filter("siteCollection/root ne null")
    .Select("siteCollection,webUrl")
    .GetAsync();

```