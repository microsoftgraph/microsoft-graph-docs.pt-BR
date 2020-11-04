---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee350a4f44f60ac50a943f670a366a5a89db24de
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903634"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/$count')
    .header('ConsistencyLevel','eventual')
    .get();

```