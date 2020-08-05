---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1fb8b554fe5db5a8023d0d6dafc497868a9fe6e4
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565785"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const store = {
  defaultLanguageTag: "en-US"
};

let res = await client.api('/termStore')
    .version('beta')
    .update(store);

```