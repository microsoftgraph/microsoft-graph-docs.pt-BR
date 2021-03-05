---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e7a29c741e6a8e361b0ee6b49678b865cd082b35
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465219"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels')
    .version('beta')
    .filter('membershipType eq \'private\'')
    .get();

```