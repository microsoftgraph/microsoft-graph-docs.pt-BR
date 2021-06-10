---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 925275c3ca30a44c53a3eef50d8509be2e25799d
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869120"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleDefinitions = await client.api('/roleManagement/cloudPC/roleDefinitions')
    .version('beta')
    .get();

```