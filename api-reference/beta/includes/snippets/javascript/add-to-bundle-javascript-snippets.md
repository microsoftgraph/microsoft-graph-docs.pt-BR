---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6a621138945be8bb963907f1ec34d65862aecdf9
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932587"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  id: "123456!87"
};

let res = await client.api('/drive/bundles/{bundle-id}/children')
    .version('beta')
    .post({driveItem : driveItem});

```