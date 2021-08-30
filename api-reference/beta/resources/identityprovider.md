---
title: Tipo de recurso do identityProvider
description: Representa os provedores de identidade em um locatário do Azure Active Directory e em um locatário do Azure AD B2C.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: a04c5fcf709da10a1b7b1c37d4d81097e656bc4a
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695305"
---
# <a name="identityprovider-resource-type-deprecated"></a>Tipo de recurso do identityProvider (preterido)
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

Representa provedores de identidade com [Identidades externas](/azure/active-directory/external-identities/) para locatário do Azure Active Directory e um locatário do Azure AD B2C.

Para cenários do Azure AD B2B em um locatário do Microsoft Azure Active Directory, o tipo de provedor de identidade pode ser o Google ou o Facebook.

A configuração de um provedor de identidade no locatário do Microsoft Azure Active Directory permite novos cenários de convidado no Azure AD B2B. Por exemplo, uma organização possui recursos no Microsoft 365 que precisam ser compartilhados com um usuário do Gmail. O usuário do Gmail usará as credenciais de conta do Google para autenticar e acessar os documentos.

Em um locatário do Azure Active Directory B2C, o tipo de provedor de identidade pode ser **Microsoft**, **Google**, **Facebook**, **Amazon**, **LinkedIn**, **Twitter** ou qualquer [openIdConnectProvider](../resources/openidconnectprovider.md). Os seguintes provedores de identidade estão em visualização: **Weibo**, **QQ**, **WeChat** e **GitHub**.

A configuração de um provedor de identidade no locatário do Azure AD B2C permite que os usuários se inscrevam e entrem usando uma conta social ou um provedor personalizado suportado pelo OpenID Connect em um aplicativo. Por exemplo, um aplicativo pode usar o Azure AD B2C para permitir que os usuários se inscrevam no serviço usando uma conta do Facebook ou o seu próprio provedor de identidade personalizado que esteja em conformidade com o protocolo OIDC.

Se for um provedor de identidade personalizado do OpenID Connect `OpenIDConnect` como `type` será representado usando o tipo de recurso [openIdConnectProvider](../resources/openidconnectprovider.md),que herdará do tipo de recurso identityProvider.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/identityprovider-list.md)|conjunto identityProvider|Recupere todos os provedores de identidade configurados em um locatário.|
|[Criar](../api/identityprovider-post-identityproviders.md)|identityProvider|Crie um novo provedor de identidade.|
|[Obter](../api/identityprovider-get.md) |identityProvider|Recupere as propriedades de um provedor de identidade.|
|[Atualizar](../api/identityprovider-update.md)|Nenhum(a)|Atualize um provedor de identidade.|
|[Delete](../api/identityprovider-delete.md)|Nenhum(a)|Exclua um provedor de identidade.|
|[Listar os tipos de provedor disponíveis](../api/identityprovider-list-availableprovidertypes.md)|Coleção de cadeias de caracteres|Recupere todos os tipos de provedor de identidade disponíveis.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|A ID do cliente para o aplicativo obtida ao registrar o aplicativo no provedor de identidade. Este é um campo necessário. Necessário. Não anulável.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade. Isso é somente para gravar. Uma operação de leitura retornará `****`. Esse é um campo obrigatório. Obrigatório. Não anulável.|
|id|Cadeia de caracteres|O ID do provedor de identidade.|
|nome|Cadeia de caracteres|O nome de exibição do provedor de identidade. Não anulável.|
|tipo|Cadeia de caracteres|O tipo de provedor de identidade é um campo obrigatório. Para o cenário B2B:`Google`, `Facebook`. Para o cenário B2B: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`,`QQ`, `WeChat`, `OpenIDConnect`. Não anulável.|

### <a name="where-to-get-the-client-id-and-secret"></a>Como obter o ID e segredo do cliente

Cada provedor de identidade tem um processo para criar um registro do aplicativo. Por exemplo, os usuários criam um registro de aplicativo com o Facebook no [developers.facebook.com](https://developers.facebook.com/). A ID do cliente resultante e o segredo do cliente podem ser passados para [criar identityProvider](../api/identityprovider-post-identityproviders.md). Em seguida, cada objeto de usuário no diretório pode ser federado para qualquer um dos provedores de identidade do locatário para autenticação. Isso permite que o usuário entre por meio de credenciais na página de entrada do provedor de identidade. O token do provedor de identidade é validado pelo Azure AD antes que o locatário emita um token ao aplicativo.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```json
{
    "id": "String",
    "type": "String",
    "name": "String",
    "clientId": "String",
    "clientSecret": "String"
}
```
