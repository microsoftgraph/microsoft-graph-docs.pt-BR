---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3bd4a0f6aac83337a2d61852ac16847d28ae75f8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980604"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryAudit directoryAudit = graphClient.auditLogs().directoryAudits("{id}")
    .buildRequest()
    .get();

```