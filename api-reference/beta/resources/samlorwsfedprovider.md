---
title: Tipo de recurso samlOrWsFedProvider
description: Detalhes de configuração para configurar um saml ou WS-Fed de identidade baseada.
author: namkedia
localization_priority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9dbe48d7d2c229132dfea4b84282cadcdbcc8d7c
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697018"
---
# <a name="samlorwsfedprovider-resource-type"></a>Tipo de recurso samlOrWsFedProvider

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo abstrato que fornece detalhes de configuração para configurar um SAML ou WS-Fed provedor de identidade baseado em domínio externo (IdP).

Herdado de [identityProviderBase](../resources/identityproviderbase.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição do provedor de identidade baseado em SAML/WS-Fed. Herdado de [identityProviderBase](../resources/identityproviderbase.md).|
|id|Cadeia de caracteres|O identificador do provedor de identidade. Herdado da [entidade](../resources/entity.md).|
|issuerUri|Cadeia de caracteres|URI do emissor do servidor de federação.|
|metadataExchangeUri|Cadeia de caracteres|URI do ponto de extremidade do exchange de metadados usado para autenticação de aplicativos cliente ricos.|
|passiveSignInUri|Cadeia de caracteres|URI para os quais os clientes baseados na Web são direcionados ao entrar nos serviços Azure Active Directory (Azure AD).|
|metadataExchangeUri|Cadeia de caracteres|URI do ponto de extremidade do exchange de metadados usado para autenticação de aplicativos cliente ricos.|
|passiveSignInUri|Cadeia de caracteres|URI para os quais os clientes baseados na Web são direcionados ao entrar nos serviços do Azure AD.|
|preferredAuthenticationProtocol|Cadeia de caracteres|Protocolo de autenticação preferencial. Os valores com suporte incluem `saml` ou `wsfed` .|
|signingCertificate|Cadeia de caracteres|Certificado atual usado para assinar tokens passados para o plataforma de identidade da Microsoft. O certificado é formatado como uma cadeia de caracteres codificada base64 da parte pública do certificado de assinatura de token do IdP federado e deve ser compatível com a classe X509Certificate2.  <br/><br/> Essa propriedade é usada nos seguintes cenários: <ul><li> se uma rolagem for necessária fora da atualização de rolagem automática <li>um novo serviço de federação está sendo criado <li> se o novo certificado de assinatura de token não estiver presente nas propriedades de federação após a atualização do certificado de serviço de federação. </ul> <br/><br/> O Azure AD atualiza certificados por meio de um processo de autorollover no qual tenta recuperar um novo certificado dos metadados do serviço de federação, 30 dias antes da expiração do certificado atual. Se um novo certificado não estiver disponível, o Azure AD monitorará os metadados diariamente e atualizará as configurações de federação para o domínio quando um novo certificado estiver disponível.|

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
