---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c255be1ef884c9b195f7e1a0f3d238247b5c694cbb276a4001d343da7b93248e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273592"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ownedDevices = await client.api('/me/ownedDevices')
    .get();

```