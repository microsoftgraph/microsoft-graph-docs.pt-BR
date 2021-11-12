---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 888ee4b793ecf3c51e5ec597be13b744aed0e4a5ae569496bb170d5fef587d9f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/mailFolders/delta')
    .version('beta')
    .get();

```