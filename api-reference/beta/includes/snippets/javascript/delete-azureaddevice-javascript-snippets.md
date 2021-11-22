---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef0ac8e37a30b4d636263cfb7bdd5530e78b17b532608d409a730228db873f81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159573"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/admin/windows/updates/updatableAssets/{azureADDeviceId}')
    .version('beta')
    .delete();

```