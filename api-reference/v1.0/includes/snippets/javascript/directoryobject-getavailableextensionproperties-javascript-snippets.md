---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe198e42da642ccf8ed54224fffb80240fcb6e0b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779629"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extensionProperty = {
  isSyncedFromOnPremises: 'Boolean'
};

await client.api('/directoryObjects/getAvailableExtensionProperties')
    .post(extensionProperty);

```