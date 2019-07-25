---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60dd5db03a9eb2993c6b702cf14ccd6d5c1c0692
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890383"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MessageRule messageRule = graphClient.me().mailFolders("inbox").messageRules("AQAAAJ5dZqA=")
    .buildRequest()
    .get();

```