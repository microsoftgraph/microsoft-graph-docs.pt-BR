---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba80bbc07c5ee091291fb0b1f0225b534b754b945ba8a91c5cd0011df4fdf68c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157409"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let resources = await client.api('/education/classes/11012/assignments/19002/resources')
    .version('beta')
    .get();

```