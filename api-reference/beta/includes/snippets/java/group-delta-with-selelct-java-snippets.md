---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5605bcbc409f7c08f4b2161510a0a9ebece37336dedb2e026e0ce10f42276aea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159674"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupDeltaCollectionPage delta = graphClient.groups()
    .delta()
    .buildRequest()
    .select("displayName,description,mailNickname")
    .get();

```