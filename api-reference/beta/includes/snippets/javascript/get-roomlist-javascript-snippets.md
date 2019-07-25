---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6e56ac1f54b22518215bf5cae985c3a97a703422
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876831"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/places/bldg1@contoso.com')
    .version('beta')
    .get();

```