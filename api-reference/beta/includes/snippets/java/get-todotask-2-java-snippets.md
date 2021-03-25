---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d913d5b14ecfb4b5086c88ae0d6408d76d50dbed
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208610"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTaskCollectionPage tasks = graphClient.me().todo().lists("35e2-35e2-721a-e235-1a72e2351a7").tasks()
    .buildRequest()
    .get();

```