---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9f6a01c3f68456cdaead7676cc2624d84e31385
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368811"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let domainNameReferences = await client.api('/domains/contoso.com/domainNameReferences')
    .get();

```