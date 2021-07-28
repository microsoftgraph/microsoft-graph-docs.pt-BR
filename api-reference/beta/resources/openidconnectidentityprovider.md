---
title: Tipo de recurso openIdConnectIdentityProvider
description: Representa provedores de identidade OpenIDConnect em um locatário Azure Active Directory B2C.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: bbdbb83f6fd1eef7acb4cadeaca174b1e45ddbfb
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580895"
---
# <a name="openidconnectidentityprovider-resource-type"></a>Tipo de recurso openIdConnectIdentityProvider
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o OpenID Conexão de identidade em um locatário Azure Active Directory B2C.

Configurar um provedor de Conexão OpenID em um locatário B2C permite que os usuários se inscrevam e se inscrevam usando seu provedor de identidade personalizado em um aplicativo.

Este tipo herdará de [identityProviderBase](../resources/identityproviderbase.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/identityproviderbase-list.md)|[Coleção identityProviderBase](../resources/identityproviderbase.md)|Recupere todos os provedores de identidade configurados em um locatário, incluindo o OpenID Conexão de identidade.|
|[Criar](../api/identityproviderbase-post-identityproviders.md)|openIdConnectIdentityProvider|Crie um novo provedor de Conexão de identidade OpenID.|
|[Get](../api/identityproviderbase-get.md) |openIdConnectIdentityProvider|Recupere propriedades de um provedor de Conexão OpenID.|
|[Atualizar](../api/identityproviderbase-update.md)|Nenhum(a)|Atualize um provedor de Conexão openid.|
|[Delete](../api/identityproviderbase-delete.md)|Nenhum|Exclua um provedor Conexão de identidade OpenID.|
|[Listar os tipos de provedor disponíveis](../api/identityproviderbase-list-availableprovidertypes.md)|Coleção de cadeias de caracteres|Recuperar todos os tipos de provedores de identidade disponíveis no locatário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|A ID do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade. Obrigatório.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade. O clientSecret tem uma dependência de **responseType**. <ul><li>Quando **responseType** é `code` , um segredo é necessário para a troca de código de auth.</li><li>Quando **responseType** é `id_token` o segredo não é necessário porque não há troca de código. O id_token é retornado diretamente da resposta de autorização.</li></ul> Isso é somente gravação. Uma operação de leitura retorna `****`.|
|id|Cadeia de caracteres|O identificador do provedor de identidade. Necessário. Herdado de [identityProviderBase](../resources/identityproviderbase.md). Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade. |
|claimsMapping|[claimsMapping](claimsmapping.md)|Depois que o provedor OIDC envia um token de ID de volta para o Azure AD, o Azure AD precisa ser capaz de mapear as declarações do token recebido para as declarações que o Azure AD reconhece e usa. Esse tipo complexo captura esse mapeamento. Obrigatório.|
|domainHint|Cadeia de caracteres|A dica de domínio pode ser usada para pular diretamente para a página de entrada do provedor de identidade especificado, em vez de fazer com que o usuário faça uma seleção entre a lista de provedores de identidade disponíveis.|
|metadataUrl|Cadeia de caracteres|A URL do documento de metadados do provedor de Conexão OpenID. Cada provedor Conexão de identidade OpenID descreve um documento de metadados que contém a maioria das informações necessárias para executar a login. Isso inclui informações como as URLs a ser usadas e o local das chaves de assinatura públicas do serviço. O documento Conexão de metadados do OpenID está sempre localizado em um ponto de extremidade que termina em `.well-known/openid-configuration` . Forneça a URL de metadados para o provedor Conexão de identidade openid que você adicionar. Somente leitura. Obrigatório.|
|responseMode|Cadeia de caracteres|O modo de resposta define o método usado para enviar dados de volta do provedor de identidade personalizado para o Azure AD B2C. Valores possíveis: `form_post` , `query` . Obrigatório.|
|responseType|Cadeia de caracteres|O tipo de resposta descreve o tipo de informação enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizado. Valores possíveis: `code` , `id_token` , `token` .  Obrigatório.|
|escopo|String|O escopo define as informações e permissões que você está procurando coletar do provedor de identidade personalizado. As solicitações Conexão OpenID devem conter o valor de escopo openid para receber o token de ID do provedor de identidade. Sem o token de ID, os usuários não podem entrar no Azure AD B2C usando o provedor de identidade personalizado. Outros escopos podem ser anexados, separados por um espaço. Para obter mais detalhes sobre as limitações de escopo, consulte [RFC6749 Seção 3.3](https://tools.ietf.org/html/rfc6749#section-3.3). Obrigatório.|

### <a name="responsemode-value"></a>valor responseMode
|Valor|Descrição|
:--------|:----------|
|form_post|Esse modo de resposta é recomendado para melhor segurança. A resposta é transmitida por meio do método HTTP POST, com o código ou token sendo codificado no corpo usando o formato application/x-www-form-urlencoded.|
|consulta|O código ou token é retornado como um parâmetro de consulta.|

### <a name="responsetype-value"></a>valor responseType
|Valor|Descrição|
:--------|:----------|
|código|Conforme o fluxo de código de autorização, um código será retornado para o Azure AD B2C. O Azure AD B2C continua a chamar o token_endpoint para trocar o código pelo token.|
|id_token|Um token de ID é retornado ao Azure AD B2C do provedor de identidade personalizado.|
|token|Um token de acesso é retornado ao Azure AD B2C do provedor de identidade personalizado. (Esse valor não é suportado pelo Azure AD B2C no momento)|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider"
} -->

```json
{
  "id": "String",
  "displayName": "String",
  "clientId": "String",
  "clientSecret": "String",
  "claimsMapping": {
      "@odata.type": "#microsoft.graph.claimsMapping",
      "userId": "String",
      "givenName": "String",
      "surname": "String",
      "email": "String",
      "displayName": "String"
  },
  "domainHint": "String",
  "metadataUrl": "String",
  "responseMode": "String",
  "responseType": "String",
  "scope": "String"
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
