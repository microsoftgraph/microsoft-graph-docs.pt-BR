---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 80494a3ed7c97438a3b5a469dfad56b858cc21aa879bcc1082ef9791ccc2cd35
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216969"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InformationProtectionLabelCollectionPage labels = graphClient.me().informationProtection().policy().labels()
    .buildRequest()
    .get();

```