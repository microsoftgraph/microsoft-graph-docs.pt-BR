---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: defedc12486264cd4b2048b3510a69c604c3eea4030fca2c3449ed0baba7e001
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217442"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organization = await client.api('/organization')
    .version('beta')
    .get();

```