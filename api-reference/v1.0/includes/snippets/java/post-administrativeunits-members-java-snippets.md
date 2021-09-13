---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60ad9282d21e1522e57ea8d8e16180d25affcf6806fe4f13810bd4dbc18bbdf4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899560"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.directory().administrativeUnits("{id}").members().references()
    .buildRequest()
    .post(directoryObject);

```