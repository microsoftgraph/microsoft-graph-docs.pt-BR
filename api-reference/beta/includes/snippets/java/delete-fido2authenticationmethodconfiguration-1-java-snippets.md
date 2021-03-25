---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab61ee85b050bfe5edb329d07c2abf2e72dcf0b4
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209712"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("fido2")
    .buildRequest()
    .delete();

```