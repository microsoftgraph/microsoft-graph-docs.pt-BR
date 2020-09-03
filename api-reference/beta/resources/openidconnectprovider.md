---
title: tipo de recurso openIdConnectProvider
description: Representa os provedores de identidade do OpenIDConnect em um locatário do Azure Active Directory B2C.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: namkedia
ms.openlocfilehash: 9a7567ee550432dc5a0d98ce9c3a6ae7c51a0160
ms.sourcegitcommit: c6e8a2097267ace4c78124be48646f9129114b26
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/03/2020
ms.locfileid: "47340006"
---
# <a name="openidconnectprovider-resource-type"></a>tipo de recurso openIdConnectProvider

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os provedores de identidade de conexão OpenID em um locatário do Azure Active Directory B2C. 

A configuração de um provedor de conexão OpenID no locatário B2C permite que os usuários se inscrevam e entrem usando seu provedor de identidade personalizado em um aplicativo.

Herda de [identityprovider](../resources/identityprovider.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/identityprovider-list.md)|conjunto identityProvider|Recupere todos os provedores de identidade configurados em um locatário.|
|[Criar](../api/identityprovider-post-identityproviders.md)|identityProvider|Crie um novo provedor de identidade de conexão OpenID.|
|[Obter](../api/identityprovider-get.md) |identityProvider|Recupere as propriedades de um provedor de identidade de conexão OpenID.|
|[Atualizar](../api/identityprovider-update.md)|Nenhum(a)|Atualize um provedor de identidade de conexão OpenID.|
|[Delete](../api/identityprovider-delete.md)|Nenhum|Excluir um provedor de identidade de conexão OpenID.|
|[Listar os tipos de provedor disponíveis](../api/identityprovider-list-availableprovidertypes.md)|Coleção de cadeias de caracteres|Recupere todos os tipos de provedor de identidade disponíveis.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|A ID do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade. Herdado de [identityprovider](../resources/identityprovider.md). Essa é uma propriedade obrigatória.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade. O clientSecret tem uma dependência em ResponseType. No caso de ResponseType = Code, um segredo é necessário para a troca de código de autenticação, mas no caso de ResponseType = id_token não é necessário porque não há troca de código, o id_token é retornado diretamente da resposta de autorização. Isso é somente gravação. Uma operação de leitura retornará "\*\*\*\*". Herdado de [identityprovider](../resources/identityprovider.md).|
|id|Cadeia de caracteres|O ID do provedor de identidade. É uma propriedade obrigatória e é somente leitura após a criação.|
|nome|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade. É uma propriedade obrigatória e é somente leitura após a criação.|
|tipo|Cadeia de caracteres|A identidade do provedor de identidade. Deve ser `OpenIDConnect` . É uma propriedade obrigatória e é somente leitura após a criação.|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|Depois que o provedor OIDC envia um token de ID de volta para o Azure AD, o Azure AD precisa ser capaz de mapear as declarações do token recebido para as declarações que o Azure AD reconhece e usa. Esse tipo complexo captura esse mapeamento. É uma propriedade necessária.|
|domainHint|String|A dica de domínio pode ser usada para saltar diretamente para a página de entrada do provedor de identidade especificado, em vez de fazer com que o usuário faça uma seleção entre a lista de provedores de identidade disponíveis.|
|metadataUrl|String|A URL do documento de metadados do provedor de identidade de conexão OpenID Connect. Cada provedor de identidade de conexão OpenID descreve um documento de metadados que contém a maioria das informações necessárias para executar a entrada. Isso inclui informações como as URLs a serem usadas e o local das chaves de assinatura pública do serviço. O documento de metadados do OpenID Connect sempre está localizado em um ponto de extremidade que termina em. well-known/OpenID-Configuration. Para o provedor de identidade de conexão OpenID que você está procurando adicionar, será necessário fornecer a URL de metadados. É uma propriedade obrigatória e é somente leitura após a criação.|
|responsemode|String|O modo de resposta define o método que deve ser usado para enviar os dados de volta do provedor de identidade personalizada para o Azure AD B2C. Os seguintes modos de resposta podem ser usados: <ul><li/>`form_post` : Este modo de resposta é recomendado para melhor segurança. A resposta é transmitida por meio do método HTTP POST, com o código ou token codificado no corpo usando o formato application/x-www-form-urlencoded.<li/>`query` : O código ou token é retornado como um parâmetro de consulta.</ul> É uma propriedade necessária.|
|responseType|String|O tipo de resposta descreve que tipo de informação é enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizada. Os seguintes tipos de resposta podem ser usados:<ul><li/> `code` : Conforme o fluxo do código de autorização, um código será retornado de volta para o Azure AD B2C. O Azure AD B2C continua a chamar o token_endpoint para trocar o código do token.<li/> `id_token` : Um token de ID retorna de volta para o Azure AD B2C do provedor de identidade personalizado. <li/>`token` : Um token de acesso retorna de volta para o Azure AD B2C do provedor de identidade personalizado. (Esse valor não é suportado pelo Azure AD B2C no momento)</ul> É uma propriedade necessária.|
|escopo|String|Escopo define as informações e permissões que você pretende coletar de seu provedor de identidade personalizado. Solicitações de conexão OpenID devem conter o valor de escopo OpenID para receber o token de ID do provedor de identidade. Sem o token de ID, os usuários não podem entrar no Azure AD B2C usando o provedor de identidade personalizado. Outros escopos podem ser acrescentados separados por espaço. Para obter mais detalhes sobre as limitações do escopo, consulte a [seção 3,3 da RFC6749](https://tools.ietf.org/html/rfc6749#section-3.3). É uma propriedade necessária.|

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
