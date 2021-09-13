---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: feda6c5e4ad99cd0de85965112ab6b31f7245014eb5935e00764461106aefde9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099307"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationalBranding organizationalBranding = new OrganizationalBranding();
organizationalBranding.signInPageText = "Default";
organizationalBranding.usernameHintText = "DefaultHint";

graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding()
    .buildRequest()
    .patch(organizationalBranding);

```