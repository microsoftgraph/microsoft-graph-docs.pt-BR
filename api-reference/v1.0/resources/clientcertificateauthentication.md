---
title: Tipo de recurso clientCertificateAuthentication
description: Representa a configuração para recuperar um clientCertificateAuthentication.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 69870b1160078495d3b9440260aab1f231041eef
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882393"
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
