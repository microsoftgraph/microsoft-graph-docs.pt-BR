---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97f3b5a8d027ed06e9c34637d494b8ade3652bfe6fe09685901bd578299b868b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329392"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage appliesTo = graphClient.policies().tokenLifetimePolicies("{id}").appliesTo()
    .buildRequest()
    .get();

```