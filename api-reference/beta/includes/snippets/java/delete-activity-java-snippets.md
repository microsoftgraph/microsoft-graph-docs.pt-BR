---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1dcb22e61a37984a5aa841aecf26f12fce743220
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983330"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().activities("13881113971988980728")
    .buildRequest()
    .delete();

```