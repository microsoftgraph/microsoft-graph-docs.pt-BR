---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: affb15d7d223b32248dc3bca0023b11bd7200b75
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316872"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcAuditEvent cloudPcAuditEvent = graphClient.deviceManagement().virtualEndpoint().auditEvents("{id}")
    .buildRequest()
    .get();

```