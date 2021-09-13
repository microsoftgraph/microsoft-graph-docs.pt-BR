---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2254e8659e19df3de0859808e0d1529d6945f49c2be28eb3b4c765ea18cbc9f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897826"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.sites("{siteId}").drive()
    .buildRequest()
    .get();

```