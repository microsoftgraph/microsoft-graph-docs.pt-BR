---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8273bcfd3e8fdbf3bbcb7d7e6672dbaca092190c51de63401ecd5c85294075a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099606"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps')
    .version('beta')
    .get();

```