---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afbcc9a4b6b2e7731789cd780afd09b903d2eac1
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997986"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/educationalActivities')
    .version('beta')
    .get();

```