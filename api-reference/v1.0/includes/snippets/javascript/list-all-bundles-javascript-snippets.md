---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe9c1636bf1805479f279f67eda411c4b9dac144
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757882"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bundles = await client.api('/drive/bundles')
    .version('beta')
    .get();

```