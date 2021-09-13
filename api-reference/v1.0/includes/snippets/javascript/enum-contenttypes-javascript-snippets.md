---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd4d85ff222fa1eb6fed7a498e0a5aee4d3c415c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026049"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contentTypes = await client.api('/sites/{site-id}/contentTypes')
    .get();

```