---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70833b42095fd88f2d5913a97ae07328de944aebfade79aae9445ea0ce6add92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217391"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskFolder = {
  name: 'Volunteer'
};

await client.api('/me/outlook/taskfolders')
    .version('beta')
    .post(outlookTaskFolder);

```