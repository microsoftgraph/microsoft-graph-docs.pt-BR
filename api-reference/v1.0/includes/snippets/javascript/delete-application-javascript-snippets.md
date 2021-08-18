---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b75d194f646369f05ecb23fb0a8846cad93993144b58414c1385003fd3a2c431
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329194"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}')
    .delete();

```