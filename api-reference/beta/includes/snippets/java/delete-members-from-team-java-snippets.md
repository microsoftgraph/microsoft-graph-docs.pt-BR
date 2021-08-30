---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3301906d5cf6bc5457c4f792f13686a31ba637cf397e241e41d044a2ae1c84b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158839"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062").members("ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=")
    .buildRequest()
    .delete();

```