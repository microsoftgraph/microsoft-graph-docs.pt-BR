---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d28a615a9d7ac87aaba6fb71ba0801e62ce94230
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970650"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().languages("{id}")
    .buildRequest()
    .delete();

```