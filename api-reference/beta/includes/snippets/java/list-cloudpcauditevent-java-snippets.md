---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff410bf39f41b1d7010da447a36501baa3ea58ba51fdea83539be2c70fea1321
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101922"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcAuditEventCollectionPage auditEvents = graphClient.deviceManagement().virtualEndpoint().auditEvents()
    .buildRequest()
    .get();

```