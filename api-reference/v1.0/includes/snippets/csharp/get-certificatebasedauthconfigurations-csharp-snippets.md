---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d51991eb077f052ac88619b95ed7798203406435dd3b0a123aed9ad836cb07c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275359"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var certificateBasedAuthConfiguration = await graphClient.Organization["{organization-id}"].CertificateBasedAuthConfiguration
    .Request()
    .GetAsync();

```