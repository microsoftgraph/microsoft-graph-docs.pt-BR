---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22fda01f45078cfc0fcc74ea85307b0647006c005e11df0bf3817f1dfd40fd80
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272277"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userCredentialUsageDetails = await graphClient.Reports.UserCredentialUsageDetails
    .Request()
    .GetAsync();

```