---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66abe262e08579cb07216de6b6681f84f0ba0c07292555d559514cf03e42897d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216809"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage ownedDevices = graphClient.me().ownedDevices()
    .buildRequest()
    .get();

```