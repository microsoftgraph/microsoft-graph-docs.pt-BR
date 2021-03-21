---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db704fb312a01aab5cce2b60e73001b17c4cf6d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974589"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CertificateBasedAuthConfiguration certificateBasedAuthConfiguration = new CertificateBasedAuthConfiguration();
LinkedList<CertificateAuthority> certificateAuthoritiesList = new LinkedList<CertificateAuthority>();
CertificateAuthority certificateAuthorities = new CertificateAuthority();
certificateAuthorities.isRootAuthority = true;
certificateAuthorities.certificate = Base64.getDecoder().decode("Binary");
certificateAuthoritiesList.add(certificateAuthorities);
certificateBasedAuthConfiguration.certificateAuthorities = certificateAuthoritiesList;

graphClient.organization("{id}").certificateBasedAuthConfiguration().references()
    .buildRequest()
    .post(certificateBasedAuthConfiguration);

```