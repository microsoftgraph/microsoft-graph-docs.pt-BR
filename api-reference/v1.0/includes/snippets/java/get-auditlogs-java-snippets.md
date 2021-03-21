---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8bda52df2bc9e1f937912c5d002426bb38498f0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968757"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuditLogRoot auditLogRoot = graphClient.auditLogs()
    .buildRequest()
    .get();

```