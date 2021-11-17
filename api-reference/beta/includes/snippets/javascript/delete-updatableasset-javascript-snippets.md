---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7746012c438a733a933e228b2d38a29ed6b05be20875204b4aa0f118b328bd29
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156393"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/admin/windows/updates/updatableAssets/{updatableAssetId}')
    .version('beta')
    .delete();

```