---
title: tipo de recurso socialIdentityProvider
description: Representa provedores de identidade social em um locatário do Azure Active Directory e um locatário do Azure AD B2C.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 6f5e01a2be28f4ba0d6021232bd0f0a1e8cdefd6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136380"
---
# <a name="socialidentityprovider-resource-type"></a>tipo de recurso socialIdentityProvider
Namespace: microsoft.graph

Representa provedores de identidade social com [Identidades externas](/azure/active-directory/external-identities/) para o locatário do Azure Active Directory (Azure AD) e um locatário do Azure AD B2C.

Herdado de [identityProviderBase](../resources/identityproviderbase.md).

Para cenários do Azure AD B2B em um locatário do Azure AD, o tipo de provedor de identidade pode ser `Google` ou `Facebook`.

A configuração de um provedor de identidade no locatário do Microsoft Azure Active Directory permite novos cenários de convidado no Azure AD B2B. Por exemplo, uma organização possui recursos no Microsoft 365 que precisam ser compartilhados com um usuário do Gmail. O usuário do Gmail usará as credenciais de conta do Google para autenticar e acessar os documentos.

Em um locatário Azure AD B2C, o tipo de provedor de identidade pode ser `Microsoft`, `Google`, `Facebook`, `Amazon`, `LinkedIn `ou `Twitter`. Os seguintes provedores de identidade estão em versão prévia: `Weibo`, `QQ`, `WeChat`e `GitHub`.

Configurar um provedor de identidade em seu locatário do Azure AD B2C permite que os usuários se inscrevam e entrem usando um provedor com suporte de conta social em um aplicativo. Por exemplo, um aplicativo pode usar o Azure AD B2C para permitir que os usuários se inscrevam no serviço usando uma conta do Facebook.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/identitycontainer-list-identityproviders.md)|Coleção [identityProviderBase](../resources/identityproviderbase.md) |Recupere todos os provedores de identidade configurados em um locatário, incluindo os tipos de objeto [socialidentityprovider](../resources/socialidentityprovider.md). Não há como recuperar apenas os provedores de identidade social em um locatário.|
|[Criar](../api/identitycontainer-post-identityproviders.md)|[socialidentityprovider](../resources/socialidentityprovider.md) |Crie um novo objeto [socialidentityprovider](../resources/socialidentityprovider.md).|
|[Get](../api/identityproviderbase-get.md) |[socialidentityprovider](../resources/socialidentityprovider.md) |Recupere propriedades de um objeto [socialidentityprovider](../resources/socialidentityprovider.md).|
|[Atualizar](../api/identityproviderbase-update.md)|Nenhum(a)|Atualize um objeto [socialidentityprovider](../resources/socialidentityprovider.md).|
|[Delete](../api/identityproviderbase-delete.md)|Nenhum|Exclua um objeto [socialidentityprovider](../resources/socialidentityprovider.md).|
|[Listar os tipos de provedor disponíveis](../api/identityproviderbase-availableprovidertypes.md)|Coleção de cadeias de caracteres|Recuperar todos os tipos de provedores de identidade disponíveis no locatário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|O identificador do aplicativo cliente obtido ao registrar o aplicativo no provedor de identidade. Necessário.|
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
