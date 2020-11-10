---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0779b6208ff720db4d7cfd6738650fb2a3d7856d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965751"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADYAAAImV_jAAA=")
    .buildRequest()
    .expand("eventMessage/event")
    .get();

```