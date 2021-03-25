---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4029a499b6077ae1ec9e433fa6cf5e6c51ee79cf
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202829"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("kim@contoso.com").authentication().microsoftAuthenticatorMethods("_jpuR-TGZtk6aQCLF3BQjA2")
    .buildRequest()
    .delete();

```