---
title: Tipo de recurso samlOrWsFedProvider
description: Detalhes de configuração para configurar um provedor de identidade baseado em SAML WS-Fed saml.
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0dec6cac2cdbe1bbe7f42d0d3580e82148e99ff3
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296578"
---
# <a name="samlorwsfedprovider-resource-type"></a>Tipo de recurso samlOrWsFedProvider

Namespace: microsoft.graph

Um tipo abstrato que fornece detalhes de configuração para configurar um SAML ou WS-Fed IdP (provedor de identidade baseado em domínio) externo.

Herdado de [identityProviderBase](../resources/identityproviderbase.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição do provedor de identidade baseado em SAML/WS-Fed. Herdado de [identityProviderBase](../resources/identityproviderbase.md).|
|id|Cadeia de caracteres|O identificador do provedor de identidade. Herdado da [entidade](../resources/entity.md).|
|issuerUri|String|URI do emissor do servidor de federação.|
|metadataExchangeUri|Cadeia de caracteres|URI do ponto de extremidade de troca de metadados usado para autenticação de aplicativos cliente avançados.|
|metadataExchangeUri|String|URI do ponto de extremidade de troca de metadados usado para autenticação de aplicativos cliente avançados.|
|passiveSignInUri|Cadeia de caracteres|URI para o qual os clientes baseados na Web são direcionados ao entrar em serviços Azure Active Directory (Azure AD).|
|preferredAuthenticationProtocol|authenticationProtocol|Protocolo de autenticação preferencial. Os valores possíveis são: `wsFed`, `saml`, `unknownFutureValue`.|
|signingCertificate|Cadeia de caracteres|Certificado atual usado para assinar tokens passados para o plataforma de identidade da Microsoft. O certificado é formatado como uma cadeia de caracteres codificada em Base64 da parte pública do certificado de assinatura de token do IdP federado e deve ser compatível com a classe X509Certificate2.  <br/><br/> Essa propriedade é usada nos seguintes cenários: <ul><li> se uma substituição for necessária fora da atualização de registro automático <li>um novo serviço de federação está sendo configurado <li> se o novo certificado de assinatura de token não estiver presente nas propriedades de federação depois que o certificado do serviço de federação tiver sido atualizado. </ul> <br/><br/> Azure AD atualiza certificados por meio de um processo de registro automático no qual ele tenta recuperar um novo certificado dos metadados do serviço de federação, 30 dias antes da expiração do certificado atual. Se um novo certificado não estiver disponível, o Azure AD monitorará os metadados diariamente e atualizará as configurações de federação para o domínio quando um novo certificado estiver disponível.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.samlOrWsFedProvider",
  "baseType": "microsoft.graph.identityProviderBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.samlOrWsFedProvider",
  "id": "String (identifier)",
  "displayName": "String",
  "issuerUri": "String",
  "metadataExchangeUri": "String",
  "signingCertificate": "String",
  "passiveSignInUri": "String",
  "preferredAuthenticationProtocol": "String"
}
```
