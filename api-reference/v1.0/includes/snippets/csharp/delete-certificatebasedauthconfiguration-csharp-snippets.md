---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49d2739bd76ebace1d0442b7ebe5ebc45c43e347e9c9852bf0c713b4b4be9e0b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272928"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Organization["{organization-id}"].CertificateBasedAuthConfiguration["{certificateBasedAuthConfiguration-id}"]
    .Request()
    .DeleteAsync();

```