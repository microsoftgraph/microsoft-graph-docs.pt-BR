---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 182a7426f87513f0b6e66db36e69cb07df3ce868102ee28b06d99bda52e56700
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160282"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage memberOf = graphClient.devices("{id}").memberOf()
    .buildRequest()
    .get();

```