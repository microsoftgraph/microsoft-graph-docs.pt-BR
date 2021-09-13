---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5a297bda3152a43e3f55e0b4eb1637eecb43470c19586f78a20a38db39304a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329273"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTaskListCollectionPage lists = graphClient.me().todo().lists()
    .buildRequest()
    .get();

```