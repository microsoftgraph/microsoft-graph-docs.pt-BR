---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2b095965cb74b95a2037d872f3ec8743985c2e3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProviders/Amazon-OAuth')
    .get();

```