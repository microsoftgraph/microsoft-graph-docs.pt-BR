---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e3001c909a9c2a14fda4515a466b5f350598071a521ec5d956b2f03567b472df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217012"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemVersion driveItemVersion = graphClient.me().drive().items("{item-id}").versions("{version-id}")
    .buildRequest()
    .get();

```