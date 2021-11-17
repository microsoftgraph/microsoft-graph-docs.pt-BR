---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0bc5715d9e4e98a88234bd4a2b361c7466aa18b8d4b98c169d6c0ff1fc0b5856
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214461"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let trustFrameworkKeySet = await client.api('/trustFramework/keySets/{id}')
    .version('beta')
    .get();

```