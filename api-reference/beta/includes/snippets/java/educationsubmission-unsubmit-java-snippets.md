---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3dda156cb52d908c62bf5442f342129c33fd24de
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955410"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11021").assignments("19002").submissions("850f51b7")
    .unsubmit()
    .buildRequest()
    .post();

```