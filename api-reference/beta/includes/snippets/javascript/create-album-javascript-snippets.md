---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4dda443535b84559a24a30d86325da52b2f1eaf6
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932626"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: "My Day at the Beach",
  "@name.conflictBehavior" : "rename",
  bundle: { album: {} },
  children: [
    { id: "1234asdf" }
  ]
};

let res = await client.api('/drive/bundles')
    .version('beta')
    .post({driveItem : driveItem});

```