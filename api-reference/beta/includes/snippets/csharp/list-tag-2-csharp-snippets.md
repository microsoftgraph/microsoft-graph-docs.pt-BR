---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ffdedc3e64ad0c16975feaae2052177cf283aa28bf65dc4395503cd7d21d2006
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216381"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childTags = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Tags["{ediscovery.tag-id}"].ChildTags
    .Request()
    .GetAsync();

```