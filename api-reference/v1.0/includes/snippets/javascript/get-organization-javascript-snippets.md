---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0e50525689853e024bbabccadaa6f25c1ac7a40
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2020
ms.locfileid: "43511145"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/organization')
    .get();

```