---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10be0eb75e6a54b63c80deab1b8411206bf5626d
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241198"
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