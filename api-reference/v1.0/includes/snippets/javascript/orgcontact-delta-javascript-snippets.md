---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6f64d265b7969a281548e48dd316ab7c1168a2dc
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082121"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/delta')
    .get();

```