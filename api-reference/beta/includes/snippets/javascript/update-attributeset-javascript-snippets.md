---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95dab8ea74fe7420a43703395de9cbd083b1ce55
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223530"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attributeSet = {
    description: 'Attributes for engineering team',
    maxAttributesPerSet: 20
};

await client.api('/directory/attributeSets/Engineering')
    .version('beta')
    .update(attributeSet);

```