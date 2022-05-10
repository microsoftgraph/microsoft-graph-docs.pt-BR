---
title: Tipo de recurso samlOrWsFedExternalDomainFederation
description: Representa uma maneira de federar seu locatário Azure AD com uma organização externa cujo provedor de identidade dá suporte ao protocolo SAML ou WS-Fed segurança.
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 80e9e4234af0e8ab234092968439124ff1aa23ea
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296581"
---
# <a name="samlorwsfedexternaldomainfederation-resource-type"></a>Tipo de recurso samlOrWsFedExternalDomainFederation

Namespace: microsoft.graph

Permite que um locatário Azure Active Directory (Azure AD) federe com uma organização externa cujo IdP (provedor de identidade) dá suporte ao protocolo SAML ou WS-Fed. Isso permite que o locatário do Azure AD dê acesso aos seus recursos para usuários convidados. Para obter mais informações sobre a federação saml ou WS-Fed IdP, consulte Federação com saml ou WS-Fed de [identidade para usuários convidados](/azure/active-directory/external-identities/direct-federation).

Herda [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar samlOrWsFedExternalDomainFederations](../api/samlorwsfedexternaldomainfederation-list.md)|[Coleção samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Obtenha uma lista dos [objetos samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) e suas propriedades.|
|[Criar samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-post.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Crie um novo [objeto samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) .|
|[Obter samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-get.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Leia as propriedades e as relações de um [objeto samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) .|
|[Atualizar samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-update.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Atualize as propriedades de um [objeto samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) .|
|[Excluir samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-delete.md)|Nenhum|Exclui um [objeto samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) .|
|[Listar domínios](../api/samlorwsfedexternaldomainfederation-list-domains.md)|[coleção externalDomainName](../resources/externaldomainname.md)|Obtenha os recursos externalDomainName da propriedade de navegação de domínios.|
|[Criar externalDomainName](../api/samlorwsfedexternaldomainfederation-post-domains.md)|[externalDomainName](../resources/externaldomainname.md)|Crie um novo objeto externalDomainName.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição do IdP WS-Fed SAML. Herdado de [identityProviderBase](../resources/identityproviderbase.md).|
|id|Cadeia de caracteres|O identificador do provedor de identidade. Herdado da [entidade](../resources/entity.md).|
|issuerUri|Cadeia de caracteres|URI do emissor do servidor de federação. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|metadataExchangeUri|String|URI do ponto de extremidade de troca de metadados usado para autenticação de aplicativos cliente avançados. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|passiveSignInUri|Cadeia de caracteres|URI para o qual os clientes baseados na Web são direcionados ao entrar Azure AD serviços. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|preferredAuthenticationProtocol|authenticationProtocol|Protocolo de autenticação preferencial. Os valores possíveis são: `wsFed`, `saml`, `unknownFutureValue`. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|signingCertificate|String|Certificado atual usado para assinar tokens passados para o plataforma de identidade da Microsoft. O certificado é formatado como uma cadeia de caracteres codificada em Base64 da parte pública do certificado de assinatura de token do IdP federado e deve ser compatível com a classe X509Certificate2.  <br/><br/> Essa propriedade é usada nos seguintes cenários: <ul><li> se uma substituição for necessária fora da atualização de registro automático <li>um novo serviço de federação está sendo configurado <li> se o novo certificado de assinatura de token não estiver presente nas propriedades de federação depois que o certificado do serviço de federação tiver sido atualizado. </ul> <br/><br/> Azure AD atualiza certificados por meio de um processo de registro automático no qual ele tenta recuperar um novo certificado dos metadados do serviço de federação, 30 dias antes da expiração do certificado atual. Se um novo certificado não estiver disponível, o Azure AD monitorará os metadados diariamente e atualizará as configurações de federação para o domínio quando um novo certificado estiver disponível. <br/><br/> Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|Domínios|[coleção externalDomainName](../resources/externaldomainname.md)|Coleção de nomes de domínio das organizações externas com as qual o locatário está federando. Suporta `$filter` (`eq`).|

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
