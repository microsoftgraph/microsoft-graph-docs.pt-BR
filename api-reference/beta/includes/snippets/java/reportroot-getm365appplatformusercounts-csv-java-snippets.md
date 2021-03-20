---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66408f4fce52cb969632ae4818b37335d0af157e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968414"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/reports/getM365AppPlatformUserCounts(period='D7')/content", InputStream.class)
    .buildRequest()
    .get();

```