---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45ff0b8fbc8eb0fb191e174e834a42c9c40710ed
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955923"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.drives("{driveId}")
    .buildRequest()
    .get();

```