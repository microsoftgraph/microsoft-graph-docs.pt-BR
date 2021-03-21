---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f63edc38cb470623c0f0628c241e232d34803aaf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984194"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Presence presence = graphClient.me().presence()
    .buildRequest()
    .get();

```