---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a37e8b59cdb05cf69e3ce62e0a5d2edb6c2ec2c4ab54697f89be7aceaa7865f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275022"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AQMkADJmMTUAAAgVZAAAA")
    .buildRequest()
    .expand("mentions")
    .get();

```