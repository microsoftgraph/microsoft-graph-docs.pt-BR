---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 14ef37c9139415596e0c8154c70f2d743f2e41208696475ead0b81747092e39c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327502"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = graphClient.me().mailFolders("AAMkAGVmMDEzN")
    .buildRequest()
    .get();

```