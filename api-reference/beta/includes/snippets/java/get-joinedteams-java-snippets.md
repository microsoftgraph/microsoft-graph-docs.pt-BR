---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28cd5fedca9e1eb75a63b4ebd466a74ef769db1eead3db4f4237cf361c509d1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217611"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamCollectionWithReferencesPage joinedTeams = graphClient.me().joinedTeams()
    .buildRequest()
    .get();

```