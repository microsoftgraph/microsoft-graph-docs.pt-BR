---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 42a6db6c17afa3c8e7dddf0e22822c2008cfd3e6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948502"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let call = await client.api('/communications/calls/{id}')
    .version('beta')
    .get();

```