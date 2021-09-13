---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f8d17d0eb444f8578d5ccf3975d05b9d0f01346814e84779b92ea50f4429504
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217569"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.identity().b2cUserFlows("B2C_1_Customer").languages("en").defaultPages("idpselections").content()
    .buildRequest()
    .get();

```