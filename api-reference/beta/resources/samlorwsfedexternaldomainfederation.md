---
title: Tipo de recurso samlOrWsFedExternalDomainFederation
description: Representa a federação SAML/WS-Fed configurada com um locatário Azure Active Directory (Azure AD)
author: namkedia
localization_priority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: aee7550d2a8a098fa841056637cfc73aed5aca03
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697016"
---
# <a name="samlorwsfedexternaldomainfederation-resource-type"></a>Tipo de recurso samlOrWsFedExternalDomainFederation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um recurso que permite que um locatário do Azure Active Directory (Azure AD) defina a federação com outra organização cujo provedor de identidade (IdP) oferece suporte ao protocolo SAML ou WS-Fed. Isso permite que o locatário do Azure AD permita que os usuários convidados acessem seus recursos. Para obter mais informações sobre a federação de IdP SAML/WS-Fed, consulte Federação com provedores de identidade [SAML/WS-Fed para usuários convidados.](/azure/active-directory/external-identities/direct-federation)

Herda [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar samlOrWsFedExternalDomainFederations](../api/samlorwsfedexternaldomainfederation-list.md)|[Coleção samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Obter uma lista dos [objetos samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) e suas propriedades.|
|[Criar samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-post.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Crie um novo [objeto samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)|
|[Obter samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-get.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Leia as propriedades e as relações de um [objeto samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)|
|[Atualizar samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-update.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Atualize as propriedades de [um objeto samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)|
|[Excluir samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-delete.md)|Nenhum|Exclui um [objeto samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)|
|[Listar domínios](../api/samlorwsfedexternaldomainfederation-list-domains.md)|[coleção externalDomainName](../resources/externaldomainname.md)|Obter os recursos externalDomainName da propriedade de navegação de domínios.|
|[Criar externalDomainName](../api/samlorwsfedexternaldomainfederation-post-domains.md)|[externalDomainName](../resources/externaldomainname.md)|Crie um novo objeto externalDomainName.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição do SAML ou WS-Fed IdP baseado. Herdado de [identityProviderBase](../resources/identityproviderbase.md).|
|id|Cadeia de caracteres|O identificador do provedor de identidade. Herdado da [entidade](../resources/entity.md).|
|issuerUri|Cadeia de caracteres|URI do emissor do servidor de federação. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|metadataExchangeUri|Cadeia de caracteres|URI do ponto de extremidade do exchange de metadados usado para autenticação de aplicativos cliente ricos. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|passiveSignInUri|Cadeia de caracteres|URI para os quais os clientes baseados na Web são direcionados ao entrar nos serviços do Azure AD. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|preferredAuthenticationProtocol|Cadeia de caracteres|Protocolo de autenticação preferencial. Os valores com suporte incluem `saml` ou `wsfed` . Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|signingCertificate|Cadeia de caracteres|Certificado atual usado para assinar tokens passados para o plataforma de identidade da Microsoft. O certificado é formatado como uma cadeia de caracteres codificada base64 da parte pública do certificado de assinatura de token do IdP federado e deve ser compatível com a classe X509Certificate2.  <br/><br/> Essa propriedade é usada nos seguintes cenários: <ul><li> se uma rolagem for necessária fora da atualização de rolagem automática <li>um novo serviço de federação está sendo criado <li> se o novo certificado de assinatura de token não estiver presente nas propriedades de federação após a atualização do certificado de serviço de federação. </ul> <br/><br/> O Azure AD atualiza certificados por meio de um processo de autorollover no qual tenta recuperar um novo certificado dos metadados do serviço de federação, 30 dias antes da expiração do certificado atual. Se um novo certificado não estiver disponível, o Azure AD monitorará os metadados diariamente e atualizará as configurações de federação para o domínio quando um novo certificado estiver disponível. <br/><br/> Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|domínios|[coleção externalDomainName](../resources/externaldomainname.md)|Coleção de nomes de domínio das organizações externas com as que o locatário está federando. Suporta `$filter` (`eq`).|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.samlOrWsFedExternalDomainFederation",
  "baseType": "microsoft.graph.samlOrWsFedProvider",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.samlOrWsFedExternalDomainFederation",
  "id": "String (identifier)",
  "displayName": "String",
  "issuerUri": "String",
  "metadataExchangeUri": "String",
  "signingCertificate": "String",
  "passiveSignInUri": "String",
  "preferredAuthenticationProtocol": "String"
}
```
