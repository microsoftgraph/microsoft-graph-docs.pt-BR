---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1083da088f73c708d8f2065497e282f74e9d079c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806079"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const audioRoutingGroup = {
  id: 'oneToOne',
  routingMode: 'oneToOne',
  sources: [
    '632899f8-2ea1-4604-8413-27bd2892079f'
  ],
  receivers: [
    '550fae72-d251-43ec-868c-373732c2704f'
  ]
};

await client.api('/communications/calls/{id}/audioRoutingGroups')
    .version('beta')
    .post(audioRoutingGroup);

```