---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1c45fb563d65ddf8214b8684345e6b8622bdeeda98f23e17eccb897bf9483582
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100967"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserDeltaCollectionPage delta = graphClient.users()
    .delta()
    .buildRequest()
    .get();

```