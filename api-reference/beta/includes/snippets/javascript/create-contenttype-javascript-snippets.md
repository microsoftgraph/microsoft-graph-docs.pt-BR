---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f53cc5364c6353d5f7783fe1988b5f3881ef2cc4
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202042"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contentType = {
    name: 'docSet',
    description: 'custom docset',
    base: {
        name: 'Document Set',
        id: '0x0120D520'
    },
    group: 'Document Set Content Types' 
};

await client.api('/sites/{id}/contentTypes')
    .version('beta')
    .post(contentType);

```