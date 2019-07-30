---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28b52051517c275f336c77ab2d85f471c38c732b
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931197"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/teamwork/installedApps/{id}/upgrade')
    .version('beta')
    .post();

```