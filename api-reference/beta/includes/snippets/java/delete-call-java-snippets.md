---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1085f7d97a772dc4d53fcb0efdffc11dfac05fb
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945464"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .buildRequest()
    .delete();

```