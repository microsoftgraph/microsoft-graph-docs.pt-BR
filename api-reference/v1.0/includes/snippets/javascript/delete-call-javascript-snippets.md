---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4260461615d7318ae7ca49d529c3a8c2330f9357
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865702"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896')
    .delete();

```