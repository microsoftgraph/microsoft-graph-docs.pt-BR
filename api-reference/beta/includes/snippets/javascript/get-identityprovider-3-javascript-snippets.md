---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 686e1c9307a7d3f33bdca2f2182cb0a8996236fc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960968"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviders = await client.api('/identityProviders')
    .version('beta')
    .get();

```