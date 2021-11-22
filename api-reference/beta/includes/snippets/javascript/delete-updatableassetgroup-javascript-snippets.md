---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ddcd4e339b971307233b241f678efdaeecfd93adeb5635220006e4aa72993176
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214439"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/admin/windows/updates/updatableAssets/{updatableAssetGroupId}')
    .version('beta')
    .delete();

```