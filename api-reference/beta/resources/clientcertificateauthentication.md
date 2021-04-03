---
title: Tipo de recurso clientCertificateAuthentication
description: Representa a configuração para buscar um clientCertificateAuthentication em uma chamada de API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0e88a1de011fb975afae49d53b8707b95e16157c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509376"
---
# <a name="clientcertificateauthentication-resource-type"></a>Tipo de recurso clientCertificateAuthentication

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo derivado de apiAuthenticationConfigurationBase que é usado para representar a autenticação de certificado de cliente baseada em Pkcs12. Isso é usado para recuperar as propriedades públicas de certificados carregados.

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
