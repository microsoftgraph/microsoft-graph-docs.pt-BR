---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5eccbb327be3dd4b72105b986230ae59280001ec
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997987"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationalActivities = await graphClient.Me.Profile.EducationalActivities
    .Request()
    .GetAsync();

```