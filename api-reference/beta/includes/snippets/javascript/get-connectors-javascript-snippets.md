---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5a1aae8be6dcacc83d11a8818e620265b2a1fcc
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945493"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/connectors')
    .version('beta')
    .get();

```