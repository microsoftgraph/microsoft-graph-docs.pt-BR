---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2cf929da0d428221b0de232e7018fa94929842fbd1c3b8c1e2c3afde4bc53cc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897850"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const changeScreenSharingRole = {
  role: 'viewer'
};

await client.api('/communications/calls/{id}/changeScreenSharingRole')
    .post(changeScreenSharingRole);

```