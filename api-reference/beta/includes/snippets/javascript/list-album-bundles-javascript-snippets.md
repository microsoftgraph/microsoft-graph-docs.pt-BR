---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce8adc56a95c4f5cca65ef25cff8ab9a8d030f241466da9e2654137fd1dd432d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157827"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bundles = await client.api('/drive/bundles?filter=bundle/album%20ne%20null')
    .version('beta')
    .filter('bundle/album ne null')
    .get();

```