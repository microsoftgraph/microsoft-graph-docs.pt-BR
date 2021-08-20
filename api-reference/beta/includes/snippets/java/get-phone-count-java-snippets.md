---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2286a7556b7496a7704ea7128a146502093b5c72a100e083ca5769ac5ad8f65c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159109"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:wa"));

OrgContactCollectionPage contacts = graphClient.contacts()
    .buildRequest( requestOptions )
    .get();

```