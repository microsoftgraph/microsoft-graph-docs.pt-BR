---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 289f252442193ce59c510d176cdabee7dda922de
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239321"
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