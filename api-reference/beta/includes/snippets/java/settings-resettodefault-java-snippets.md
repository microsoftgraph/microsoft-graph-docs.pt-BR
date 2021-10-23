---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e81ab19d434af80ac158788690a15c7d43ab11f9b7dc2bb0cc2b6fe78b0f05b7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213819"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("{caseId}").settings()
    .resetToDefault()
    .buildRequest()
    .post();

```