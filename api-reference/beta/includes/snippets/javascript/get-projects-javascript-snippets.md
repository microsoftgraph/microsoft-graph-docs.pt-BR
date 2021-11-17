---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b73546787cf9b03f3b4eee3733fcf44f98121fddbcaeb8d7f6028c36615c03e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let projects = await client.api('/me/profile/projects')
    .version('beta')
    .get();

```