---
title: Tipo de recurso x509CertificateAuthenticationMethodConfiguration
description: 'Representa os detalhes do Azure AD native Certificate-Based Authentication (CBA) no locatário, incluindo se o método de autenticação está habilitado ou desabilitado e os usuários e grupos que podem se registrar e usá-lo.'
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="x509certificateauthenticationmethodconfiguration-resource-type"></a>Tipo de recurso x509CertificateAuthenticationMethodConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes do Azure AD native Certificate-Based Authentication (CBA) no locatário, incluindo se o método de autenticação está habilitado ou desabilitado e os usuários e grupos que podem se registrar e usá-lo.

Herda de [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter x509CertificateAuthenticationMethodConfiguration](../api/x509certificateauthenticationmethodconfiguration-get.md)|[x509CertificateAuthenticationMethodConfiguration](../resources/x509certificateauthenticationmethodconfiguration.md)|Leia as propriedades e as relações de um objeto x509CertificateAuthenticationMethodConfiguration.|
|[Atualizar x509CertificateAuthenticationMethodConfiguration](../api/x509certificateauthenticationmethodconfiguration-update.md)|[x509CertificateAuthenticationMethodConfiguration](../resources/x509certificateauthenticationmethodconfiguration.md)|Atualize as propriedades de um objeto x509CertificateAuthenticationMethodConfiguration.|
|[Excluir x509CertificateAuthenticationMethodConfiguration](../api/x509certificateauthenticationmethodconfiguration-delete.md)|Nenhum| Restaure o objeto x509CertificateAuthenticationMethodConfiguration para sua configuração padrão.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador da política de método de autenticação. O valor é sempre `X509Certificate`. Herdado [da autenticaçãoMethodConfiguration](../resources/authenticationmethodconfiguration.md).|
|state|authenticationMethodState|Os valores possíveis são: `enabled`, `disabled`. Herdado [da autenticaçãoMethodConfiguration](../resources/authenticationmethodconfiguration.md).|
|certificateUserBindings|[Coleção x509CertificateUserBinding](../resources/x509certificateuserbinding.md)|Define campos no certificado X.509 que mapeiam para atributos do objeto de usuário do Azure AD para vincular o certificado ao usuário. A **prioridade** do objeto determina a ordem na qual a associação é realizada. A primeira associação que corresponde será usada e o restante ignorado. |
|authenticationModeConfiguration|[x509CertificateAuthenticationModeConfiguration](../resources/x509certificateauthenticationmodeconfiguration.md)|Define configurações de autenticação forte. Essa configuração inclui o modo de autenticação padrão e as diferentes regras para fortes vinculações de autenticação. |


## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|includeTargets|[coleção authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Uma coleção de usuários ou grupos habilitados para usar o método de autenticação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.x509CertificateAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.x509CertificateAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "certificateUserBindings": [
    {
      "@odata.type": "microsoft.graph.x509CertificateUserBinding"
    }
  ],
  "authenticationModeConfiguration": {
    "@odata.type": "microsoft.graph.x509CertificateAuthenticationModeConfiguration"
  }
}
```

