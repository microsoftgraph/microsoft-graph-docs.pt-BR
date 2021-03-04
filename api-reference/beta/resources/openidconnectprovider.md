---
title: Tipo de recurso openIdConnectProvider
description: Representa provedores de identidade OpenIDConnect em um locatário B2C do Azure Active Directory.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: cbc2e95b04ec4ce8ce3c5472a1be61e743a008fa
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444088"
---
# <a name="openidconnectprovider-resource-type"></a>Tipo de recurso openIdConnectProvider

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa provedores de identidade do OpenID Connect em um locatário do Azure Active Directory B2C. 

A configuração de um provedor OpenID Connect no locatário B2C permite que os usuários se inscrevam e se conectem usando seu provedor de identidade personalizado em um aplicativo.

Herda de [identityProvider](../resources/identityprovider.md).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/identityprovider-list.md)|conjunto identityProvider|Recupere todos os provedores de identidade configurados em um locatário.|
|[Criar](../api/identityprovider-post-identityproviders.md)|identityProvider|Crie um novo provedor de identidade do OpenID Connect.|
|[Obter](../api/identityprovider-get.md) |identityProvider|Recupere as propriedades de um provedor de identidade do OpenID Connect.|
|[Atualizar](../api/identityprovider-update.md)|Nenhum(a)|Atualize um provedor de identidade do OpenID Connect.|
|[Delete](../api/identityprovider-delete.md)|Nenhum(a)|Exclua um provedor de identidade do OpenID Connect.|
|[Listar os tipos de provedor disponíveis](../api/identityprovider-list-availableprovidertypes.md)|Coleção de cadeias de caracteres|Recupere todos os tipos de provedor de identidade disponíveis.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|A ID do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade. Herdado [de identityProvider](../resources/identityprovider.md). Essa é uma propriedade necessária.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade. O clientSecret tem uma dependência do responseType. No caso de responseType = code, um segredo é necessário para a troca de código de auth, mas no caso de responseType = id_token não é necessário porque não há troca de código, o id_token é retornado diretamente da resposta de autorização. Isso é somente gravação. Uma operação de leitura retornará "\*\*\*\*". Herdado [de identityProvider](../resources/identityprovider.md).|
|id|Cadeia de caracteres|O ID do provedor de identidade. É uma propriedade necessária e é lida somente após a criação.|
|nome|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade. É uma propriedade necessária e é lida somente após a criação.|
|type|Cadeia de caracteres|A identidade do provedor de identidade. Deve ser `OpenIDConnect` . É uma propriedade necessária e é lida somente após a criação.|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|Depois que o provedor OIDC envia um token de ID de volta para o Azure AD, o Azure AD precisa ser capaz de mapear as declarações do token recebido para as declarações que o Azure AD reconhece e usa. Esse tipo complexo captura esse mapeamento. É uma propriedade necessária.|
|domainHint|String|A dica de domínio pode ser usada para pular diretamente para a página de entrada do provedor de identidade especificado, em vez de fazer com que o usuário faça uma seleção entre a lista de provedores de identidade disponíveis.|
|metadataUrl|String|A URL do documento de metadados do provedor de identidade do OpenID Connect. Cada provedor de identidade do OpenID Connect descreve um documento de metadados que contém a maioria das informações necessárias para executar a conexão. Isso inclui informações como as URLs a ser usadas e o local das chaves de assinatura públicas do serviço. O documento de metadados do OpenID Connect está sempre localizado em um ponto de extremidade que termina em .well-known/openid-configuration . Para o provedor de identidade do OpenID Connect que você está procurando adicionar, você precisará fornecer a URL de metadados. É uma propriedade necessária e é lida somente após a criação.|
|responseMode|String|O modo de resposta define o método que deve ser usado para enviar os dados de volta do provedor de identidade personalizado para o Azure AD B2C. Os seguintes modos de resposta podem ser usados: <ul><li/>`form_post` : Este modo de resposta é recomendado para melhor segurança. A resposta é transmitida por meio do método HTTP POST, com o código ou token sendo codificado no corpo usando o formato application/x-www-form-urlencoded.<li/>`query` : O código ou token é retornado como um parâmetro de consulta.</ul> É uma propriedade necessária.|
|responseType|String|O tipo de resposta descreve que tipo de informação é enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizado. Os seguintes tipos de resposta podem ser usados:<ul><li/> `code` : De acordo com o fluxo de código de autorização, um código será retornado para o Azure AD B2C. O Azure AD B2C continua a chamar o token_endpoint para trocar o código pelo token.<li/> `id_token` : Um token de ID é retornado ao Azure AD B2C do provedor de identidade personalizado. <li/>`token` : Um token de acesso é retornado ao Azure AD B2C do provedor de identidade personalizado. (Esse valor não é suportado pelo Azure AD B2C no momento)</ul> É uma propriedade necessária.|
|escopo|String|O escopo define as informações e permissões que você está procurando coletar do provedor de identidade personalizado. As solicitações do OpenID Connect devem conter o valor de escopo openid para receber o token de ID do provedor de identidade. Sem o token de ID, os usuários não podem entrar no Azure AD B2C usando o provedor de identidade personalizado. Outros escopos podem ser anexados separados pelo espaço. Para obter mais detalhes sobre as limitações de escopo, consulte [RFC6749 Seção 3.3](https://tools.ietf.org/html/rfc6749#section-3.3). É uma propriedade necessária.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.openIdConnectProvider"
} -->

```json
{
  "id": "String",
  "name": "String",
  "type": "String",
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


