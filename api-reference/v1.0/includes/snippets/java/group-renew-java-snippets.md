---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d07e6cae5dbef1ca70416aa00288ab28120a3eef9463bcade12b7927488398bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101062"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .renew()
    .buildRequest()
    .post();

```