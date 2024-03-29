---
title: tipo de recurso socialIdentityProvider
description: Representa provedores de identidade social em um locatário do Azure Active Directory e um locatário do Azure AD B2C.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: ef47509cf1ca212d7e2e7dda9f76a1352037ba7b
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696971"
---
# <a name="socialidentityprovider-resource-type"></a>tipo de recurso socialIdentityProvider
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa provedores de identidade social com [Identidades Externas](/azure/active-directory/external-identities/) para locatários do Active Directory do Azure (Microsoft Azure Active Directory) e do Azure AD B2C.

Herdado de [identityProviderBase](../resources/identityproviderbase.md).

Para cenários do Azure AD B2B em um locatário do Microsoft Azure Active Directory, o tipo de provedor de identidade pode ser o Google ou o Facebook.

A configuração de um provedor de identidade no locatário do Microsoft Azure Active Directory permite novos cenários de convidado no Azure AD B2B. Por exemplo, uma organização possui recursos no Microsoft 365 que precisam ser compartilhados com um usuário do Gmail. O usuário do Gmail usará as credenciais de conta do Google para autenticar e acessar os documentos.

Em um locatário do Azure AD B2C, o tipo de provedor de identidade pode ser Microsoft, Google, Facebook, Amazon, LinkedIn ou Twitter. Os seguintes provedores de identidade estão em visualização: Weibo, QQ, WeChat e GitHub.

Configurar um provedor de identidade em seu locatário do Azure AD B2C permite que os usuários se inscrevam e entrem usando um provedor com suporte de conta social em um aplicativo. Por exemplo, um aplicativo pode usar o Azure AD B2C para permitir que os usuários se inscrevam no serviço usando uma conta do Facebook.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/identitycontainer-list-identityproviders.md)|Coleção [identityProviderBase](../resources/identityproviderbase.md) |Recupere todos os provedores de identidade configurados em um locatário, incluindo os tipos de objeto [socialIdentityProvider](../resources/socialidentityprovider.md). Não há como recuperar apenas os provedores de identidade social em um locatário.|
|[Criar](../api/identitycontainer-post-identityproviders.md)|socialidentityprovider |Crie um novo objeto [ socialIdentityProvider ](../resources/socialidentityprovider.md).|
|[Obter](../api/identityproviderbase-get.md) |socialidentityprovider |Recupere propriedades de um objeto [socialIdentityProvider](../resources/socialidentityprovider.md).|
|[Atualizar](../api/identityproviderbase-update.md)|Nenhum(a)|Atualize um objeto [socialIdentityProvider](../resources/socialidentityprovider.md).|
|[Delete](../api/identityproviderbase-delete.md)|Nenhum|Exclua um objeto [socialIdentityProvider](../resources/socialidentityprovider.md).|
|[Listar os tipos de provedor disponíveis](../api/identityproviderbase-availableprovidertypes.md)|Coleção de cadeias de caracteres|Recuperar todos os tipos de provedores de identidade disponíveis no locatário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|O identificador de cliente do aplicativo obtido ao registrar o aplicativo com o provedor de identidade. Obrigatório.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo obtido quando o aplicativo é registrado com o provedor de identidade. Isso é somente gravação. Uma operação de leitura retorna `****`. Obrigatório.|
|id|Cadeia de caracteres|O identificador do provedor de identidade. Herdado de [identityProviderBase](../resources/identityproviderbase.md). Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade. Herdado de [identityProviderBase](../resources/identityproviderbase.md).|
|identityProviderType|Cadeia de caracteres|Para um cenário B2B, valores possíveis: `Google`, `Facebook`. Para um cenário B2C, valores possíveis: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`. Obrigatório.|

### <a name="where-to-get-the-client-identifier-and-secret"></a>Onde obter o identificador e o segredo do cliente

Cada provedor de identidade tem um processo para criar um registro do aplicativo. Por exemplo, os usuários criam um registro de aplicativo com o Facebook no [developers.facebook.com](https://developers.facebook.com/). O identificador do cliente e o segredo do cliente resultantes podem ser passados para [criar identityProvider](../api/identitycontainer-post-identityproviders.md). Em seguida, cada objeto de usuário no diretório pode ser federado para qualquer um dos provedores de identidade do locatário para autenticação. Isso permite que o usuário entre inserindo credenciais na página de entrada do provedor de identidade. O token do provedor de identidade é validado pelo Azure AD antes que o locatário emita um token ao aplicativo.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.socialIdentityProvider"
} -->

```json
{
    "id": "String",
    "identityProviderType": "String",
    "displayName": "String",
    "clientId": "String",
    "clientSecret": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "socialIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
