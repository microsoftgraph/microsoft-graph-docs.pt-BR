---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8bb9117842f10c908447c787b987d5fe33e72ac273323129376eced8af73026
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273001"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var credentialUserRegistrationDetails = await graphClient.Reports.CredentialUserRegistrationDetails
    .Request()
    .GetAsync();

```