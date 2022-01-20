---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a9ee9f214a7fe2dbbfb8f8607cdcb618846aaf4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113334"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .renew()
    .buildRequest()
    .post();

```