---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5973aa8964709117de332a07432f275f87dae8d5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793686"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/directoryObjects/{id}')
    .get();

```