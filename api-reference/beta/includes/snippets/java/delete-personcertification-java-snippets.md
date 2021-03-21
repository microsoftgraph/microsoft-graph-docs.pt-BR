---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e20fac713320cb2e5bb6829fdb0aa8642e4ba903
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979205"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{userId}").profile().certifications("{id}")
    .buildRequest()
    .delete();

```