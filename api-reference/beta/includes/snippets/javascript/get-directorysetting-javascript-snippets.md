---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a4628589420ed7a599b4af6e595c0a3cd8c938e
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514390"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directorySetting = await client.api('/settings/f0b2d6f5-097d-4177-91af-a24e530b53cc')
    .version('beta')
    .get();

```