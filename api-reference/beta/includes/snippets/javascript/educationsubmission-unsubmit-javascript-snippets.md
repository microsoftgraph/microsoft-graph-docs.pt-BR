---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a09642727057acf8abe711605f5e54666ac5623b4cf47d3c2c112e8e0cf4c7c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156795"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit')
    .version('beta')
    .post();

```