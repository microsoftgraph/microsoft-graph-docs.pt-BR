---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e3dbbdcd7bca5ea80f98cfd5ab2db97271b9fdd4efefa214b0b63419161ee0e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900115"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MessageCollectionPage messages = graphClient.me().mailFolders("{id}").messages()
    .buildRequest()
    .get();

```