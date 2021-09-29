---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66ad63d96d423f88293827e8e22e254f34e7034d
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996243"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/default/bannerLogo", InputStream.class)
    .buildRequest()
    .get();

```