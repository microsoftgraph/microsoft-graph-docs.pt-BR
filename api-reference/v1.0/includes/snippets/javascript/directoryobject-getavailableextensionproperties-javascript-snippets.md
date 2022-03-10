---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b99939eee9cf002520e441f0b6af1a2ed5e61b2
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410988"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extensionProperty = {
  isSyncedFromOnPremises: true
};

await client.api('/directoryObjects/getAvailableExtensionProperties')
    .post(extensionProperty);

```