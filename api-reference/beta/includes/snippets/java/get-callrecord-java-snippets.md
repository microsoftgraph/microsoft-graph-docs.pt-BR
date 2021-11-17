---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 543811db06c404f1b288d1f317f65b116240af928b541086b280a79c79e3a78c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899436"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CallRecord callRecord = graphClient.communications().callRecords("{id}")
    .buildRequest()
    .get();

```