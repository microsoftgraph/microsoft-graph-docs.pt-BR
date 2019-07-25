---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 778a82b8785195b6d06a58e7a5473016c4f6b1c9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884707"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

graphClient.me().messages("{id}")
    .replyAll(comment)
    .buildRequest()
    .post();

```