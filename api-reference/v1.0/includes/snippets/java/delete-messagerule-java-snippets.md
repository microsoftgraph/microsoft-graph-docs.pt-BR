---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8ed2bdcbf95d6f4d7c8ab0103385400280170b9887c6d6449741802c8e37eac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274799"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().mailFolders("inbox").messageRules("AQAAAJ5dZp8=")
    .buildRequest()
    .delete();

```