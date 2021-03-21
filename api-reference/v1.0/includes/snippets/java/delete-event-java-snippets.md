---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1a0f7b4309b5f93b53d652eb518d334e07499b0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978023"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().events("{id}")
    .buildRequest()
    .delete();

```