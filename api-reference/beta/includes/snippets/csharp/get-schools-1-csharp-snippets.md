---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8694da534295eaadcd5e7e665570fdcbd72bc553
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951590"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schools = await graphClient.Education.Classes["{educationClass-id}"].Schools
    .Request()
    .GetAsync();

```