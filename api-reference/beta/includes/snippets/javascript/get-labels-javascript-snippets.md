---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 16b046b3883df9d48a1d4cf2dafc4d16dadf5329
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994379"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/informationprotection/policy/labels')
    .version('beta')
    .get();

```