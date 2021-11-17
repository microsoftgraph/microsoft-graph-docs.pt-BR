---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96880df8482f3f9a19e248cb5e18c693b1c0a0133862285d1a517212e7fe9107
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159741"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let updatableAsset = await client.api('/admin/windows/updates/updatableAssets/{updatableAssetId}')
    .version('beta')
    .get();

```