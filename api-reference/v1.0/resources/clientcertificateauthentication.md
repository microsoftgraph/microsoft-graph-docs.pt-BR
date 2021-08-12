---
title: Tipo de recurso clientCertificateAuthentication
description: Representa a configuração para recuperar um clientCertificateAuthentication.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 89214a0e9c6805adc7bafa59f12b0091c89c953d4380bf3ea9b95d89ade2973b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212134"
---
# <a name="clientcertificateauthentication-resource-type"></a>Tipo de recurso clientCertificateAuthentication

Namespace: microsoft.graph

Um tipo derivado de apiAuthenticationConfigurationBase usado para representar uma autenticação de certificado cliente baseada em Pkcs12. Isso é usado para recuperar as propriedades públicas de certificados carregados.

Herda de [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|certificateList| [Coleção pkcs12CertificateInformation](../resources/pkcs12CertificateInformation.md)| A lista de certificados carregados para este conector de API.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.clientCertificateAuthentication"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
  "certificateList": "Collection(microsoft.graph.pkcs12CertificateInformation)",
}
```
