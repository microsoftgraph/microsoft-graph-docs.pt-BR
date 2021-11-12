---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 633e8e8b363452bb0e10a90dcf1a26ef4f0fe590b1dae08d674f8d3be3150c66
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376682"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserCollectionWithReferencesPage allowedUsers = graphClient.print().shares("{printerShareId}").allowedUsers()
    .buildRequest()
    .get();

```