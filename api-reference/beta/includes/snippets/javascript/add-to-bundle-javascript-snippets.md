---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 783ef7e16656ca908bf3f01eaf7c287eb160e70f1f2e0383cf1ef0b11defdb91
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  id: '123456!87'
};

await client.api('/drive/bundles/{bundle-id}/children')
    .version('beta')
    .post(driveItem);

```