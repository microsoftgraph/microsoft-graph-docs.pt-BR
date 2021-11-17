---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0f598571331a0ba563df9f8faf99fb9536def9d9a3c10b01ec2c6fb3d72c0a35
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899164"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationMethod authenticationMethod = graphClient.me().authentication().methods("{id}")
    .buildRequest()
    .get();

```