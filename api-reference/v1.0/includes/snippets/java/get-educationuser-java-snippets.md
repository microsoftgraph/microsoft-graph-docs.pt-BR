---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9473a8fb9e69473229b96000f5866499e960afd0
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945964"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = graphClient.education().me().user()
    .buildRequest()
    .get();

```