---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6a99c53088dc53fa8e276794304233e695547ae6cb636c0988ef20c49c741e6b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156338"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcUserSetting cloudPcUserSetting = graphClient.deviceManagement().virtualEndpoint().userSettings("556092f8-92f8-5560-f892-6055f8926055")
    .buildRequest()
    .get();

```