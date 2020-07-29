---
title: tipo de recurso openIdConnectProvider
description: Representa os provedores de identidade do OpenIDConnect em um locatário do Azure Active Directory B2C.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: namkedia
ms.openlocfilehash: 0331870d54c5fd46c2239d48d4136252660681f9
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509914"
---
# <a name="openidconnectprovider-resource-type"></a>tipo de recurso openIdConnectProvider

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os provedores de identidade de conexão OpenID em um locatário do Azure Active Directory B2C. 

A configuração de um provedor de conexão OpenID no locatário B2C permite que os usuários se inscrevam e entrem usando seu provedor de identidade personalizado em um aplicativo.

Herda de [identityprovider](../resources/identityprovider.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|A ID do cliente do aplicativo obtido ao registrar o aplicativo com o provedor de identidade. Herdado de [identityprovider](../resources/identityprovider.md). Essa é uma propriedade obrigatória.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo obtido ao registrar o aplicativo com o provedor de identidade. O clientSecret tem uma dependência em ResponseType. No caso de ResponseType = Code, um segredo é necessário para a troca de código de autenticação, mas no caso de ResponseType = id_token não é necessário porque não há troca de código, o id_token é retornado diretamente da resposta de autorização. Isso é somente gravação. Uma operação de leitura retornará "\*\*\*\*". Herdado de [identityprovider](../resources/identityprovider.md).|
|id|String|O ID do provedor de identidade. É uma propriedade obrigatória e é somente leitura após a criação.|
|nome|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade. É uma propriedade obrigatória e é somente leitura após a criação.|
|tipo|Cadeia de caracteres|A identidade do provedor de identidade. Deve ser `OpenIDConnect` . É uma propriedade obrigatória e é somente leitura após a criação.|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|Depois que o provedor OIDC envia um token de ID de volta para o Azure AD, o Azure AD precisa ser capaz de mapear as declarações do token recebido para as declarações que o Azure AD reconhece e usa. Esse tipo complexo captura esse mapeamento. É uma propriedade necessária.|
|domainHint|Cadeia de caracteres|A dica de domínio pode ser usada para saltar diretamente para a página de entrada do provedor de identidade especificado, em vez de fazer com que o usuário faça uma seleção entre a lista de provedores de identidade disponíveis.|
|metadataUrl|Cadeia de caracteres|A URL do documento de metadados do provedor de identidade de conexão OpenID Connect. Cada provedor de identidade de conexão OpenID descreve um documento de metadados que contém a maioria das informações necessárias para executar a entrada. Isso inclui informações como as URLs a serem usadas e o local das chaves de assinatura pública do serviço. O documento de metadados do OpenID Connect sempre está localizado em um ponto de extremidade que termina em. well-known/OpenID-Configuration. Para o provedor de identidade de conexão OpenID que você está procurando adicionar, será necessário fornecer a URL de metadados. É uma propriedade obrigatória e é somente leitura após a criação.|
|responsemode|Cadeia de caracteres|O modo de resposta define o método que deve ser usado para enviar os dados de volta do provedor de identidade personalizada para o Azure AD B2C. Os seguintes modos de resposta podem ser usados: <ul><li/>`form_post`: Este modo de resposta é recomendado para melhor segurança. A resposta é transmitida por meio do método HTTP POST, com o código ou token codificado no corpo usando o formato application/x-www-form-urlencoded.<li/>`query`: O código ou token é retornado como um parâmetro de consulta.</ul> É uma propriedade necessária.|
|responseType|Cadeia de caracteres|O tipo de resposta descreve que tipo de informação é enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizada. Os seguintes tipos de resposta podem ser usados:<ul><li/> `code`: Conforme o fluxo do código de autorização, um código será retornado de volta para o Azure AD B2C. O Azure AD B2C continua a chamar o token_endpoint para trocar o código do token.<li/> `id_token`: Um token de ID retorna de volta para o Azure AD B2C do provedor de identidade personalizado. <li/>`token`: Um token de acesso retorna de volta para o Azure AD B2C do provedor de identidade personalizado. (Esse valor não é suportado pelo Azure AD B2C no momento)</ul> É uma propriedade necessária.|
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
