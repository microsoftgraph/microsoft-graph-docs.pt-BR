---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0581999fbac9b75e8646e2aa5e269b8f8c5c25dc84b297b9e2dc0c13b5ef0802
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329360"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage registeredDevices = graphClient.me().registeredDevices()
    .buildRequest()
    .get();

```