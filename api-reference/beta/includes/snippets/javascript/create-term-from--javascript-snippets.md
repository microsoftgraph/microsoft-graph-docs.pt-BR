---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 319ea0f350e641af2bf9c63caf6355a5c5fa3b2ff85950d1bddd53ea407e948e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099491"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const term = {
  labels: [
    {
      languageTag: 'en-US',
      name: 'Car',
      isDefault: true
    }
  ]
};

await client.api('/termStore/sets/{setId}/terms')
    .version('beta')
    .post(term);

```