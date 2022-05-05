---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6edc7c676050670572984016908966dd99d90a2a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220195"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bundles = await client.api('/drive/bundles?filter=bundle/album%20ne%20null')
    .filter('bundle/album ne null')
    .get();

```