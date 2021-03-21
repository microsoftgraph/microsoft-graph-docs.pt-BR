---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12fed7e5cb57bcf109475502a813c5d2821eeaa4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977708"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.drives("{drive-id}")
    .buildRequest()
    .get();

```