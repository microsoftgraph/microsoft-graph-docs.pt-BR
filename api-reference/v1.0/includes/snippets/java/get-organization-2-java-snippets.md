---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f16c990d6281badebcad9c261f7218724902b3f5
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209856"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationCollectionPage organization = graphClient.organization()
    .buildRequest()
    .get();

```