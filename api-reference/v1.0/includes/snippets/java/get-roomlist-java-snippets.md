---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 68249223c54298a9ee9f13de9ca04615a93e6b45d7b24ba04656998902d283fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406871"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Place place = graphClient.places("bldg1@contoso.com")
    .buildRequest()
    .get();

```