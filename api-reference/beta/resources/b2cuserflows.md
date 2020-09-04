---
title: Tipo de recurso b2cUserFlows
description: Representa um fluxo de usuário em um locatário do Azure Active Directory B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: e540f5b6ff21efd4ba904ddaf4dcb4868df75eff
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319658"
---
# <a name="b2cuserflows-resource-type"></a>Tipo de recurso b2cUserFlows

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um fluxo de usuário em um locatário do Azure Active Directory B2C.

Para ajudar você a configurar as tarefas de identidade mais comuns para seus aplicativos, o Azure Active Directory B2C inclui políticas configuráveis e predefinidas, chamadas [fluxos de usuário](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-overview). Um fluxo de usuário permite que você determine como os usuários interagem com o seu aplicativo quando eles fazem logon, inscrevem-se, editam um perfil ou redefinem uma senha. Você pode criar muitos fluxos de usuário de tipos diferentes em seu locatário e usá-lo em seus aplicativos, conforme necessário. Com os fluxos de usuário, você pode controle os seguintes recursos:

- Tipos de conta usados para fazer logon, como contas sociais, como uma conta local ou do Facebook
- Atributos a serem coletados do consumidor, como o nome, CEO e número do calçado
- Autenticação de vários fatores do Azure
- Personalização da interface do usuário
- Informações recebidas pelo aplicativo no token

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar fluxos de usuário](../api/b2cuserflows-list.md)|Coleção b2cUserFlow|Recuperar todos os fluxos de usuário.|
|[Obter fluxo de usuário](../api/b2cuserflows-get.md)|b2cUserFlow|Recuperar as propriedades de um fluxo de usuário.|
|[Criar fluxo de usuário](../api/b2cuserflow-post-b2cuserflows.md)|b2cUserFlow|Criar um novo fluxo de usuário.|
|[Excluir fluxo de usuário](../api/b2cuserflows-delete.md)|Nenhum|Excluir um fluxo de usuário.|
|[Listar os provedores de identidade](../api/b2cuserflows-list-identityproviders.md)|Coleção [identityProvider](../resources/identityProvider.md)|Recuperar todos os provedores de identidade em um fluxo de usuário.|
|[Adicionar provedor de identidade](../api/b2cuserflows-update-identityprovider.md)|Nenhum|Adicionar um provedor de identidade a um fluxo de usuário.|
|[Excluir provedor de identidade](../api/b2cuserflows-delete-identityprovider.md)|Nenhum|Excluir um provedor de identidade de um fluxo de usuário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|O nome do fluxo de usuário. Esse é um valor obrigatório e imutável após sua criação. O nome será antecedido pelo valor de `B2C_1_` após a criação.|
|userFlowType|Cadeia de caracteres|O [tipo de fluxo de usuário](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-versions). Os valores com suporte para **userFlowType** são:<br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwnerPasswordCredentialSignIn`</li>|
|userFlowVersion|Único|A versão do fluxo de usuário.|

## <a name="relationships"></a>Relações

| Relação       | Tipo  |Descrição|
|:---------------|:--------|:----------|
|identityProviders|Coleção [identityProvider](../resources/identityprovider.md)|Os provedores de identidade incluídos no fluxo de usuário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow",
  "optionalProperties": [],
  "keyProperty": "id"
} -->

```json
{
    "id": "String (identifier)",
    "userFlowType": "String",
    "userFlowTypeVersion": "Single",
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}]
}
```
