---
title: Tipo de recurso clientCertificateAuthentication
description: Representa a configuração para recuperar um clientCertificateAuthentication.
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 70a3885d313f368c71ab1dc2f10c158a726ffde9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109266"
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
