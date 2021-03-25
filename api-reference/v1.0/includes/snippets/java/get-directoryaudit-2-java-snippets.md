---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18f6c036ca93145dfed85a3209642654501271e1
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209543"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryAuditCollectionPage directoryAudits = graphClient.auditLogs().directoryAudits()
    .buildRequest()
    .get();

```