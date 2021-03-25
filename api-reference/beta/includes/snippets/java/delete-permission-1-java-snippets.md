---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e91d9852185c9b1ed188a361b7c57b18c73a5784
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208269"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{item-id}").permissions("{perm-id}")
    .buildRequest()
    .delete();

```