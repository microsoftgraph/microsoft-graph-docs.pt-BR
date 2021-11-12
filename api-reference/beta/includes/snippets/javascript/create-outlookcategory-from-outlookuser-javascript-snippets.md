---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5293d9b9a3966ddf19a777dc52df886251603ff1cff87d8e3b4b11b100eddf9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookCategory = {
      displayName: 'Project expenses',
      color: 'preset9'
};

await client.api('/me/outlook/masterCategories')
    .version('beta')
    .post(outlookCategory);

```