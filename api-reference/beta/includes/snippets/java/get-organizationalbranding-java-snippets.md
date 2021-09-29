---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21d445d2ea570bcb07f00160017aad45108c90be
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996247"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationalBranding organizationalBranding = graphClient.organization("84841066-274d-4ec0-a5c1-276be684bdd3").branding()
    .buildRequest()
    .get();

```