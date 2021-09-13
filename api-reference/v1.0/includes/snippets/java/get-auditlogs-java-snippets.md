---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77343d3de46c1e9cbb5826b4c4b470b234e7dd3560345a2622e2ed4f77457e20
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329969"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuditLogRoot auditLogRoot = graphClient.auditLogs()
    .buildRequest()
    .get();

```