---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa60781ffea1314f03da4823d5d7c18eb78a2790
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210082"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage appliesTo = graphClient.policies().tokenLifetimePolicies("{id}").appliesTo()
    .buildRequest()
    .get();

```