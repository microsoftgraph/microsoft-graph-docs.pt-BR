---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03071a1e2e39d87ebd09ee7cfc6639d3e499b4b5d357cffe520df0e647dfbe8a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216390"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemCollectionPage children = graphClient.drives("{drive-id}").items("{item-id}").children()
    .buildRequest()
    .get();

```