---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0323c218abad95b3f6d5c03b82573df4ce482d9da1705fbd56f51f0da0ff7338
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272658"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceHealthIssue serviceHealthIssue = graphClient.admin().serviceAnnouncement().issues("MO226784")
    .buildRequest()
    .get();

```