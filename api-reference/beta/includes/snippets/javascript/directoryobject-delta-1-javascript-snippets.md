---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2adafd97d9deb59d811972459e93c0b07e9ca131
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/directoryObjects/delta')
    .version('beta')
    .header('Prefer','return=minimal')
    .get();

```