---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23eeeb0689c79f15e815d2debc40e94698e4f26f54bd153ca6d6c8dda0da1c5c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157698"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/es-ES')
    .version('beta')
    .delete();

```