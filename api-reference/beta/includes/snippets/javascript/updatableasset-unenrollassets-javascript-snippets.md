---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ad307d25338e2af4874474986c16afe500bc6db2fe1c19ce09e39c925edd223
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275436"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unenrollAssets = {
  updateCategory: 'String',
  assets: [
    {
      '@odata.type': '#microsoft.graph.windowsUpdates.azureADDevice',
      id: 'String (identifier)'
    }
  ]
};

await client.api('/admin/windows/updates/updatableAssets/unenrollAssets')
    .version('beta')
    .post(unenrollAssets);

```