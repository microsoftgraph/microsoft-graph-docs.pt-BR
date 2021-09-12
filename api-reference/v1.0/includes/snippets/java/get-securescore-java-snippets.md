---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 317c4b3aa753e5a8c1e3913178b025f24d325c3e7f184c7195664f7049cde690
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156284"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecureScore secureScore = graphClient.security().secureScores("{id}")
    .buildRequest()
    .get();

```