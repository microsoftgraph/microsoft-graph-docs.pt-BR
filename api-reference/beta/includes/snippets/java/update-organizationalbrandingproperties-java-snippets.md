---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2c2bbd8a979c9322adc5f1e5613ab45b7fdb7b19
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179440"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationalBranding organizationalBranding = new OrganizationalBranding();
organizationalBranding.backgroundColor = "#FFFF33";

graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding()
    .buildRequest()
    .put(organizationalBranding);

```