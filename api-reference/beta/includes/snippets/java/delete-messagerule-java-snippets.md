---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26a6b4df68f6373fe3fe0a0789b9ba331ad6df30
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879337"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().mailFolders("inbox").messageRules("AQAAAJ5dZp8=")
    .buildRequest()
    .delete();

```