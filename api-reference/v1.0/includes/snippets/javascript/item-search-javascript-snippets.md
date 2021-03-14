---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1abdcdf6ebbd8e73a6c6a83718e697d77c53842d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779863"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let search = await client.api('/me/drive/root/search(q='Contoso Project')')
    .get();

```