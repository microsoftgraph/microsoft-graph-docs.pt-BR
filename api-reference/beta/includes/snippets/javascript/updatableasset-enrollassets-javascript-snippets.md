---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2213cf43a28528d8297a493313a5d1f2a1b7912ca1600f7f2a30d0d834a04fcd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101919"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const enrollAssets = {
  updateCategory: 'String',
  assets: [
    {
      '@odata.type': '#microsoft.graph.windowsUpdates.azureADDevice',
      id: 'String (identifier)'
    }
  ]
};

await client.api('/admin/windows/updates/updatableAssets/enrollAssets')
    .version('beta')
    .post(enrollAssets);

```