---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b90ed823222ac6511a1aea2a297978d4726265bf1d3809b40d0c08ce8ca1ae09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var licenseDetails = await graphClient.Me.LicenseDetails
    .Request()
    .GetAsync();

```