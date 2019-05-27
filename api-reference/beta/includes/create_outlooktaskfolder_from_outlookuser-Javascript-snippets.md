---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd5f436d26cb3d60c492d089ba8c32204e8c8833
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440055"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskFolder = {
  name: "Volunteer"
};

let res = await client.api('/me/outlook/taskfolders')
    .version('beta')
    .post({outlookTaskFolder : outlookTaskFolder});

```