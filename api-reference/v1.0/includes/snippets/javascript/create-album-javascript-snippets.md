---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f37b252e92002bc3f8872ee9dd90eada416cbbaa
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757664"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: 'My Day at the Beach',
  '@microsoft.graph.conflictBehavior': 'rename',
  bundle: { album: {} },
  children: [
    { id: '1234asdf' }
  ]
};

await client.api('/drive/bundles')
    .version('beta')
    .post(driveItem);

```