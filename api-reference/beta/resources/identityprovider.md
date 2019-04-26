---
title: Tipo de recurso do identityProvider
description: Representa um provedor de identidade do Azure Active Directory (Azure AD). O provedor de identidade pode ser Microsoft, Google, Facebook, Amazon ou LinkedIn.
localization_priority: Normal
ms.openlocfilehash: 616f4d30bf6b5aad0bb97a732cf3aaf27e0fd26d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333700"
---
# <a name="identityprovider-resource-type"></a>Tipo de recurso do identityProvider

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um provedor de identidade do Azure Active Directory (Azure AD). O provedor de identidade pode ser Microsoft, Google, Facebook, Amazon ou LinkedIn.

A configuração de um provedor de identidade em seu locatário do Azure AD B2C permite:

* Os usuários se inscrevem e entram usando uma conta social em um aplicativo de consumidor. Por exemplo, um aplicativo pode usar o Azure AD B2C para permitir que os usuários se inscrevam no serviço usando uma conta do Facebook.
* Os usuários vinculem uma conta local existente a uma conta social em um aplicativo de consumidor. Por exemplo, um usuário criou um nome de usuário e senha (conta local) no aplicativo. Mais tarde o usuário decide conectar a conta local para suas contas do Facebook, para que ele possa entrar usando o Facebook.

Configurar um provedor de identidade em seu locatário do Azure AD permite cenários futuros de usuários B2B. Por exemplo, uma organização tem recursos no Office 365 que precisam ser compartilhados com um usuário do Gmail. O usuário do Gmail usará as credenciais de conta do Google para autenticar e acessar os documentos.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter identityProvider](../api/identityprovider-get.md) |identityProvider|Recuperar as propriedades de um identityProvider existente.|
|[Criar identityProvider](../api/identityprovider-post-identityproviders.md)|identityProvider|Crie um novo identityProvider.|
|[Atualizar identityProvider](../api/identityprovider-update.md)|Nenhum|Atualize um identityProvider existente.|
|[Excluir identityProvider](../api/identityprovider-delete.md)|Nenhum|Excluir o identityProvider existente.|
|[Lista identityProviders](../api/identityprovider-list.md)|conjunto identityProvider|Lista todos os identityProviders configurados do diretório.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Obrigatório|Anulável|Descrição|
|:---------------|:--------|:--------|:--------|:----------|
|clientId|String|Sim|Não|ID do cliente para o aplicativo. Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.|
|clientSecret|String|Sim|Não|O segredo do cliente para o aplicativo. Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade. Isso é somente para gravar. Uma operação de leitura retornará "\*\*\*\*".|
|id|String|Não|Não|O ID do provedor de identidade.|
|nome|String|Não|Não|O nome de exibição exclusivo do provedor de identidade.|
|tipo|String|Sim|Não|A identidade do provedor de identidade. Deve ser um dos seguintes valores: <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook</ul>|

### <a name="where-to-get-the-client-id-and-secret"></a>Como obter o ID e segredo do cliente

Cada provedor de identidade tem um processo para criar um registro do aplicativo. Por exemplo, os usuários criam um registro de aplicativo com o Facebook no [developers.facebook.com](https://developers.facebook.com/). A ID do cliente resultante e o segredo do cliente podem ser passados para [criar identityProvider](../api/identityprovider-post-identityproviders.md). Em seguida, cada objeto de usuário no diretório pode ser federado para qualquer um dos provedores de identidade do locatário para autenticação. Isso permite que o usuário entre por meio de credenciais na página de entrada do provedor de identidade. O token do provedor de identidade é validado pelo Azure AD antes que o locatário emita um token ao aplicativo.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.IdentityProvider"
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
