---
title: Tipo de recurso openIdConnectIdentityProvider
description: Representa provedores de identidade OpenIDConnect em um locatário Azure Active Directory B2C.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: bb905d7c8cfa4842e1feb34acaa5b5f7210b50a9
ms.sourcegitcommit: f99dc2b6c8b4cb6f9f74cd780dccc47a2bccfaa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2021
ms.locfileid: "58667889"
---
# <a name="openidconnectidentityprovider-resource-type"></a>Tipo de recurso openIdConnectIdentityProvider
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os provedores Conexão de identidade do OpenID em um locatário B2C Azure Active Directory (Azure AD).

Configurar um provedor de Conexão OpenID em um locatário do Azure AD B2C permite que os usuários se inscrevam e se inscrevam em qualquer aplicativo usando seu provedor de identidade personalizado.

Herdado de [identityProviderBase](../resources/identityproviderbase.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/identitycontainer-list-identityproviders.md)|[Coleção identityProviderBase](../resources/identityproviderbase.md)|Recupere todos os provedores de identidade configurados em um locatário, incluindo o tipo de objeto [openIdConnectIdentityProvider.](../resources/openidconnectidentityprovider.md) Não há como recuperar apenas os provedores de identidade Conexão OpenID em um locatário.|
|[Create](../api/identitycontainer-post-identityproviders.md)|[openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md)|Crie um novo [objeto openIdConnectIdentityProvider.](../resources/openidconnectidentityprovider.md)|
|[Get](../api/identityproviderbase-get.md) |openIdConnectIdentityProvider|Recupere propriedades de um [objeto openIdConnectIdentityProvider.](../resources/openidconnectidentityprovider.md)|
|[Atualizar](../api/identityproviderbase-update.md)|Nenhum(a)|Atualize [um objeto openIdConnectIdentityProvider.](../resources/openidconnectidentityprovider.md)|
|[Delete](../api/identityproviderbase-delete.md)|Nenhum|[Exclua um objeto openIdConnectIdentityProvider.](../resources/openidconnectidentityprovider.md)|
|[Listar os tipos de provedor disponíveis](../api/identityproviderbase-availableprovidertypes.md)|Coleção de cadeias de caracteres|Recuperar todos os tipos de provedores de identidade disponíveis no locatário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|O identificador de cliente do aplicativo obtido ao registrar o aplicativo com o provedor de identidade. Obrigatório.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade. O clientSecret tem uma dependência de **responseType**. <ul><li>Quando **responseType** é `code` , um segredo é necessário para a troca de código de auth.</li><li>Quando **responseType** é `id_token` o segredo não é necessário porque não há troca de código. O id_token é retornado diretamente da resposta de autorização.</li></ul> Isso é somente gravação. Uma operação de leitura retorna `****`.|
|id|String|O identificador do provedor de identidade. Necessário. Herdado de [identityProviderBase](../resources/identityproviderbase.md). Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade. |
|claimsMapping|[claimsMapping](claimsmapping.md)|Depois que o provedor OIDC envia um token de ID de volta para o Azure AD, o Azure AD precisa ser capaz de mapear as declarações do token recebido para as declarações que o Azure AD reconhece e usa. Esse tipo complexo captura esse mapeamento. Obrigatório.|
|domainHint|Cadeia de caracteres|A dica de domínio pode ser usada para pular diretamente para a página de entrada do provedor de identidade especificado, em vez de fazer com que o usuário faça uma seleção entre a lista de provedores de identidade disponíveis.|
|metadataUrl|String|A URL do documento de metadados do provedor de Conexão OpenID. Cada provedor Conexão de identidade OpenID descreve um documento de metadados que contém a maioria das informações necessárias para executar a login. Isso inclui informações como as URLs a ser usadas e o local das chaves de assinatura públicas do serviço. O documento Conexão de metadados do OpenID está sempre localizado em um ponto de extremidade que termina em `.well-known/openid-configuration` . Forneça a URL de metadados para o provedor Conexão de identidade openid que você adicionar. Somente leitura. Obrigatório.|
|responseMode|[openIdConnectResponseMode](#openidconnectresponsemode-values)|O modo de resposta define o método usado para enviar dados de volta do provedor de identidade personalizado para o Azure AD B2C. Valores possíveis: `form_post` , `query` . Obrigatório.|
|responseType|[openIdConnectResponseTypes](#openidconnectresponsetypes-values)|O tipo de resposta descreve o tipo de informação enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizado. Valores possíveis: `code` , `id_token` , `token` .  Obrigatório.|
|escopo|String|O escopo define as informações e permissões que você está procurando coletar do provedor de identidade personalizado. As solicitações Conexão OpenID devem conter o valor de escopo openid para receber o token de ID do provedor de identidade. Sem o token de ID, os usuários não podem entrar no Azure AD B2C usando o provedor de identidade personalizado. Outros escopos podem ser anexados, separados por um espaço. Para obter mais detalhes sobre as limitações de escopo, consulte [RFC6749 Seção 3.3](https://tools.ietf.org/html/rfc6749#section-3.3). Obrigatório.|

### <a name="openidconnectresponsemode-values"></a>Valores openIdConnectResponseMode
|Member|Descrição|
:--------|:----------|
|form_post|Esse modo de resposta é recomendado para melhor segurança. A resposta é transmitida por meio do método HTTP POST, com o código ou token sendo codificado no corpo usando o formato application/x-www-form-urlencoded.|
|consulta|O código ou token é retornado como um parâmetro de consulta.|
|unknownFutureValue|Um valor de sentinela para indicar valores futuros.|

### <a name="openidconnectresponsetypes-values"></a>Valores openIdConnectResponseTypes
|Member|Descrição|
:--------|:----------|
|código|Conforme o fluxo de código de autorização, um código será retornado para o Azure AD B2C. O Azure AD B2C continua a chamar o token_endpoint para trocar o código pelo token.|
|id_token|Um token de ID é retornado ao Azure AD B2C do provedor de identidade personalizado.|
|token|Um token de acesso é retornado ao Azure AD B2C do provedor de identidade personalizado. (Esse valor não é suportado pelo Azure AD B2C no momento)|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
  "baseType": "microsoft.graph.identityProviderBase",
} -->

```json
{
  "@odata.type": "#microsoft.graph.openIdConnectIdentityProvider",
  "id": "String (identifier)",
  "displayName": "String",
  "clientId": "String",
  "clientSecret": "String",
  "scope": "String",
  "metadataUrl": "String",
  "domainHint": "String",
  "responseType": "String",
  "responseMode": "String",
  "claimsMapping": {
    "@odata.type": "microsoft.graph.claimsMapping"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "openidconnectIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
