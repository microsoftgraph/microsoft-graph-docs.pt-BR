---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 640393c34b9a5e9247c3f411e8069ff97e6820562a1802bb5f6fc7aad0c76781
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159588"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/trustFramework/keySets/{id}')
    .version('beta')
    .delete();

```