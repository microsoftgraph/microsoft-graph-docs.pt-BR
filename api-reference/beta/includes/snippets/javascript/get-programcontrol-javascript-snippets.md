---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5ca32deb8329916196f05674dcc062a00479bb9de0070089c54d51213430c38c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275449"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let programControls = await client.api('/programControls')
    .version('beta')
    .get();

```