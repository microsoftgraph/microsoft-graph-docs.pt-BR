---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3769c4f56a9a30a626faaedcc7c358abefed586b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/contacts/{id}/manager')
    .get();

```