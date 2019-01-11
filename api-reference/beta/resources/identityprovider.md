---
title: tipo de recurso de identityProvider
description: Representa um provedor de identidade do Windows Azure Active Directory (AD Azure). O provedor de identidade pode ser Microsoft, Google, Amazon ou Facebook, LinkedIn.
localization_priority: Normal
ms.openlocfilehash: 0a465b1c7b4ad7f74e6357e77da3692d64294e7e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858538"
---
# <a name="identityprovider-resource-type"></a>tipo de recurso de identityProvider

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um provedor de identidade do Windows Azure Active Directory (AD Azure). O provedor de identidade pode ser Microsoft, Google, Amazon ou Facebook, LinkedIn.

Configurando um provedor de identidade no seu locatário do Windows Azure AD B2C permite:

* Usuários Inscreva-se e entrar usando uma conta social em um aplicativo de consumidor. Por exemplo, um aplicativo pode usar o Windows Azure AD B2C para permitir que usuários Inscreva-se para o serviço usando uma conta do Facebook.
* Aos usuários vincular um local existente conta para uma conta social em um aplicativo de consumidor. Por exemplo, um usuário tiver criado um nome de usuário e uma senha (conta local) no aplicativo. O usuário mais tarde decide vincular a conta local existente a sua conta do Facebook, de forma que eles podem entrar usando o Facebook.

Configurando um provedor de identidade no seu locatário do Azure AD permite cenários de convidado B2B futuros. Por exemplo, uma organização tem recursos no Office 365 que precisam ser compartilhados com um usuário do Gmail. O usuário do Gmail usarão suas credenciais de conta do Google para autenticar e acessar os documentos.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter identityProvider](../api/identityprovider-get.md) |identityProvider|Leia as propriedades de um identityProvider existente.|
|[Criar identityProvider](../api/identityprovider-post-identityproviders.md)|identityProvider|Crie um novo identityProvider.|
|[Atualizar identityProvider](../api/identityprovider-update.md)|Nenhum|Atualize uma identityProvider existente.|
|[Excluir identityProvider](../api/identityprovider-delete.md)|Nenhum|Exclua um identityProvider existente.|
|[Lista identityProviders](../api/identityprovider-list.md)|coleção identityProvider|Liste todos os identityProviders configurados em um locatário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Obrigatório|Anulável|Descrição|
|:---------------|:--------|:--------|:--------|:----------|
|clientId|Cadeia de caracteres|Sim|Não|A identificação do cliente para o aplicativo. Esta é a ID de cliente obtida ao registrar o aplicativo com o provedor de identidade.|
|clientSecret|Cadeia de caracteres|Sim|Não|O segredo do cliente para o aplicativo. Esse é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade. Isso é somente gravação. Uma operação de leitura retornará "\*\*\*\*".|
|id|Cadeia de caracteres|Não|Não|A identificação do provedor de identidade.|
|name|Cadeia de caracteres|Não|Não|O nome de exibição do provedor de identidade.|
|type|Cadeia de caracteres|Sim|Não|O tipo de provedor de identidade. Ele deve ser um dos seguintes valores: <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook</ul>|

### <a name="where-to-get-the-client-id-and-secret"></a>Onde obter o cliente ID e segredo

Cada provedor de identidade tem um processo para criar um registro de aplicativo. Por exemplo, os usuários criar um registro de aplicativo com o Facebook em [developers.facebook.com](https://developers.facebook.com/). O ID de cliente resultante e segredo do cliente podem ser passados para [criar identityProvider](../api/identityprovider-post-identityproviders.md). Em seguida, cada objeto de usuário no diretório pode ser federado a qualquer um dos provedores de identidade de locatário para autenticação. Isso permite que o usuário entrar, inserindo credenciais na página de entrada do provedor de identidade. O token do provedor de identidade é validado pelo Windows Azure AD antes do locatário emite um token para o aplicativo.

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
