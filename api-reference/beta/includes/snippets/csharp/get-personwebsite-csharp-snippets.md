---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c84edb9903ab9d38c17b7409da49415a29828489
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997178"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personWebsite = await graphClient.Me.Profile.Websites["{id}"]
    .Request()
    .GetAsync();

```