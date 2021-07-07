---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1ffc69ae29e5e7fa539c7731e2fae43696e75cc2
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316564"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcAuditEventCollectionPage auditEvents = graphClient.deviceManagement().virtualEndpoint().auditEvents()
    .buildRequest()
    .get();

```