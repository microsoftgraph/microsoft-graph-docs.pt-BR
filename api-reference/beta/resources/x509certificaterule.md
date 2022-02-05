---
title: Tipo de recurso x509CertificateRule
description: Define as regras de configuração de autenticação fortes para o certificado X.509. As regras são configuradas além do modo de autenticação.
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="x509certificaterule-resource-type"></a>Tipo de recurso x509CertificateRule

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define as regras de configuração de autenticação fortes para o certificado X.509. As regras são configuradas além do modo de autenticação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|identificador|Cadeia de caracteres| O identificador do certificado X.509. Obrigatório.|
|x509CertificateAuthenticationMode|x509CertificateAuthenticationMode| O tipo de modo de autenticação forte. Os valores possíveis são: `x509CertificateSingleFactor`, `x509CertificateMultiFactor`, `unknownFutureValue`. Obrigatório.|
|x509CertificateRuleType|x509CertificateRuleType| O tipo da regra de configuração do modo de certificado X.509. Os valores possíveis são: `issuerSubject`, `policyOID`, `unknownFutureValue`. Obrigatório.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.x509CertificateRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.x509CertificateRule",
  "x509CertificateRuleType": "String",
  "identifier": "String",
  "x509CertificateAuthenticationMode": "String"
}
```

