---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8bb79072e0fcf29ec420177e4de362d467008797
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967669"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteSection onenoteSection = new OnenoteSection();
onenoteSection.displayName = "Section name";

graphClient.me().onenote().notebooks("{id}").sections()
    .buildRequest()
    .post(onenoteSection);

```