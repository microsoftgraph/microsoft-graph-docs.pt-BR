---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a21cb6760d8eab85ac24550e6f02a1fb1451711da6fa2f5f649ac925af87f1a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216604"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().deletedItems("46cc6179-19d0-473e-97ad-6ff84347bbbb")
    .restore()
    .buildRequest()
    .post();

```