---
title: Tipo de recurso x509CertificateAuthenticationModeConfiguration
description: Define as configurações de autenticação forte para o certificado X.509. Essa configuração inclui o modo de autenticação padrão e as diferentes regras de fortes vinculações de autenticação.
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="x509certificateauthenticationmodeconfiguration-resource-type"></a>Tipo de recurso x509CertificateAuthenticationModeConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define as configurações de autenticação forte para o certificado X.509. Essa configuração inclui o modo de autenticação padrão e as diferentes regras de fortes vinculações de autenticação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rules|[Coleção x509CertificateRule](../resources/x509certificaterule.md)| As regras são configuradas além do modo de autenticação para vincular um **x509CertificateRuleType** específico a **um x509CertificateAuthenticationMode**. Por exemplo, ata o `policyOID` identificador ao modo `1.32.132.343` de `x509CertificateMultiFactor` autenticação.|
|x509CertificateAuthenticationDefaultMode|x509CertificateAuthenticationMode| O tipo de modo de autenticação forte. Os valores possíveis são: `x509CertificateSingleFactor`, `x509CertificateMultiFactor`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.x509CertificateAuthenticationModeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.x509CertificateAuthenticationModeConfiguration",
  "x509CertificateAuthenticationDefaultMode": "String",
  "rules": [
    {
      "@odata.type": "microsoft.graph.x509CertificateRule"
    }
  ]
}
```

