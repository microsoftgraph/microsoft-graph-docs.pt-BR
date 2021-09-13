---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48f55881779c33a0e00748ffe7c0e072fd381c1ce06417266c60ded1694ad912
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327475"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding()
    .buildRequest()
    .delete();

```