---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8bb79072e0fcf29ec420177e4de362d467008797
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879003"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteSection onenoteSection = new OnenoteSection();
onenoteSection.displayName = "Section name";

graphClient.me().onenote().notebooks("{id}").sections()
    .buildRequest()
    .post(onenoteSection);

```