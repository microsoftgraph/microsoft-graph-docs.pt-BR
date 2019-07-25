---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61e7b09a8384a25c673620a37c8aea42542563f7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862502"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryAudit directoryAudit = graphClient.auditLogs().directoryAudits("{id}")
    .buildRequest()
    .get();

```