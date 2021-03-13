---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4d51aed24a2c89bc7fb846cfefe2ccf0074f9063
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797081"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directorySettingTemplate = await client.api('/directorySettingTemplates/{id}')
    .version('beta')
    .get();

```