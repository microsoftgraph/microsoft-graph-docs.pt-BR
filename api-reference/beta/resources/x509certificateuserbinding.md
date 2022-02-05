---
title: Tipo de recurso x509CertificateUserBinding
description: Define os campos no certificado X.509 que mapeiam para atributos do objeto de usuário do Azure AD para vincular o certificado à conta de usuário.
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="x509certificateuserbinding-resource-type"></a>Tipo de recurso x509CertificateUserBinding

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define os campos no certificado X.509 que mapeiam para atributos do objeto de usuário do Azure AD para vincular o certificado à conta de usuário.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Prioridade|Int32|A prioridade da associação. O Azure AD usa a associação com a prioridade mais alta. Esse valor deve ser um inteiro não negativo e exclusivo na coleção de objetos na propriedade **certificateUserBindings** de um **objeto x509CertificateAuthenticationMethodConfiguration** . Obrigatório|
|userProperty|String|Define a propriedade de usuário do Azure AD do objeto de usuário a ser usado para a associação. Os valores possíveis são: **userPrincipalName**, `onPremisesUserPrincipalName`, `email`. Obrigatório.|
|x509CertificateField|Cadeia de caracteres|O campo no certificado X.509 a ser usado para a associação. Os valores possíveis são: `PrincipalName`, `RFC822Name`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.x509CertificateUserBinding"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.x509CertificateUserBinding",
  "x509CertificateField": "String",
  "userProperty": "String",
  "priority": "Integer"
}
```

