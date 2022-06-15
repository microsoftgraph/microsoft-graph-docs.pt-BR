---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2052e85dbe5f212d4430463bf85bef476495d0c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092449"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteSource siteSource = new SiteSource();
Site site = new Site();
site.webUrl = "https://m365x809305.sharepoint.com/sites/Retail";
siteSource.site = site;

graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").custodians("0053a61a3b6c42738f7606791716a22a").siteSources()
    .buildRequest()
    .post(siteSource);

```