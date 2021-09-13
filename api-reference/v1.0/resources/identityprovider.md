---
title: Tipo de recurso do identityProvider
description: Representa um provedor de identidade do Azure Active Directory (Azure AD).
ms.localizationpriority: high
author: namkedia
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e6ccc49df5a96f3a7ebf16917e8eec3f075a61b3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118649"
---
# <a name="identityprovider-resource-type-deprecated"></a>Tipo de recurso do identityProvider (preterido)
Namespace: microsoft.graph

[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

Representa um provedor de identidade do Azure Active Directory (Azure AD). O provedor de identidade pode ser **Microsoft**, **Google**, **Facebook**,**Amazon**, **LinkedIn** ou **Twitter**. Os seguintes provedores de identidade estão em visualização: **Weibo**, **QQ**, **WeChat**,**GitHub** e qualquer provedor compatível com OpenID Connect. 

Configurar um provedor de identidade em seu locatário do Azure AD B2C permite que os usuários:

* Inscrevam-se e entrem usando uma conta social em um aplicativo de cliente. Por exemplo, um aplicativo pode usar o Azure AD B2C para permitir que os usuários se inscrevam no serviço usando uma conta do Facebook.
* Vincule uma conta local para uma conta em um aplicativo cliente social. Por exemplo, um usuário criou um nome de usuário e senha (conta local) no aplicativo. Mais tarde o usuário decide conectar a conta local para suas contas do Facebook, para que ele possa entrar usando o Facebook.

Configurar um provedor de identidade em seu locatário do Azure AD permite cenários futuros de usuários B2B. Por exemplo, uma organização possui recursos no Microsoft 365 que precisam ser compartilhados com um usuário do Gmail. O usuário do Gmail usará as credenciais de conta do Google para autenticar e acessar os documentos.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter identityProvider](../api/identityprovider-get.md) |identityProvider|Recuperar as propriedades de um identityProvider existente.|
|[Criar identityProvider](../api/identityprovider-post-identityproviders.md)|identityProvider|Crie um novo identityProvider.|
|[Atualizar identityProvider](../api/identityprovider-update.md)|Nenhum|Atualize um identityProvider existente.|
|[Excluir identityProvider](../api/identityprovider-delete.md)|Nenhum|Excluir o identityProvider existente.|
|[Lista identityProviders](../api/identityprovider-list.md)|conjunto identityProvider|Lista todos os identityProviders configurados do diretório.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:--------|
|clientId|Cadeia de caracteres|A ID do cliente do aplicativo. Essa é a ID do cliente obtida ao registrar o aplicativo no provedor de identidade. Necessário. Não anulável.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo. Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade. Isso é somente para gravar. Uma operação de leitura retornará `****`.  Obrigatório. Não anulável.|
|id|Cadeia de caracteres|O ID do provedor de identidade.|
|nome|Cadeia de caracteres|O nome de exibição do provedor de identidade. Não anulável.|
|tipo|Cadeia de caracteres|O tipo de provedor de identidade é um campo obrigatório. Para o cenário B2B:`Google`, `Facebook`. Para o cenário B2C: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`, `OpenIDConnect`. Não anulável.|

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
