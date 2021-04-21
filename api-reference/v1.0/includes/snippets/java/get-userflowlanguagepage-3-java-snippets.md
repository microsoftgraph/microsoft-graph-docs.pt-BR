---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28fb20a75e011a14365622c5aa6b0b7a67887739
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920457"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.identity().b2xUserFlows("B2X_1_Partner").languages("en").defaultPages("idpselections").content()
    .buildRequest()
    .get();

```