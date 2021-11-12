---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c06a80ef6307dca0b250b5534456387fa668a60e89f5874821619d145fac90e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214305"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().connectors("{printConnectorId}")
    .buildRequest()
    .delete();

```