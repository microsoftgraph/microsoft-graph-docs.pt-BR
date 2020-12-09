---
title: tipo de recurso b2cIdentityUserFlow
description: Representa um fluxo de usuário em um locatário do Azure Active Directory B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 61c3a206ee07eb7e8474e501f9064a20c6cc3840
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581086"
---
# <a name="b2cidentityuserflow-resource-type"></a>tipo de recurso b2cIdentityUserFlow

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um fluxo de usuário em um locatário do Azure Active Directory B2C.

Para ajudar você a configurar as tarefas de identidade mais comuns para seus aplicativos, o Azure Active Directory B2C inclui políticas configuráveis e predefinidas, chamadas [fluxos de usuário](/azure/active-directory-b2c/user-flow-overview). Um fluxo de usuário permite que você determine como os usuários interagem com o seu aplicativo quando eles fazem logon, inscrevem-se, editam um perfil ou redefinem uma senha. Você pode criar muitos fluxos de usuário de tipos diferentes em seu locatário e usá-lo em seus aplicativos, conforme necessário. Com os fluxos de usuário, você pode controle os seguintes recursos:

- Tipos de conta usados para fazer logon, como contas sociais, como uma conta local ou do Facebook
- Atributos a serem coletados do consumidor, como o nome, CEO e número do calçado
- Autenticação de vários fatores do Azure
- Personalização da interface do usuário
- Informações recebidas pelo aplicativo no token

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar fluxos de usuário](../api/identitycontainer-list-b2cuserflows.md)|Coleção b2cIdentityUserFlow|Recupere todos os fluxos de usuário B2C.|
|[Obter fluxo de usuário](../api/b2cidentityuserflow-get.md)|b2cIdentityUserFlow|Recupere as propriedades de um fluxo de usuário B2C.|
|[Criar fluxo de usuário](../api/identitycontainer-post-b2cuserflows.md)|b2cIdentityUserFlow|Crie um novo fluxo de usuário B2C.|
|[Excluir fluxo de usuário](../api/b2cidentityuserflow-delete.md)|Nenhum|Exclua um fluxo de usuário B2C.|
|[Listar os provedores de identidade](../api/b2cidentityuserflow-list-identityproviders.md)|Coleção [identityProvider](../resources/identityProvider.md)|Recupere todos os provedores de identidade em um fluxo de usuário B2C.|
|[Adicionar provedor de identidade](../api/b2cidentityuserflow-post-identityproviders.md)|Nenhum|Adicione um provedor de identidade a um fluxo de usuário B2C.|
|[Remover provedor de identidade](../api/b2cidentityuserflow-delete-identityproviders.md)|Nenhum|Remova um provedor de identidade de um fluxo de usuário B2C.|
|[Listar as atribuições de atributo de usuário](../api/b2cidentityuserflow-list-userattributeassignments.md)|Coleção[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) |Recupere todas as atribuições de atributos do usuário em um fluxo de usuário B2C.|
|[Criar uma tarefa de atributo de usuário](../api/b2cidentityuserflow-post-userattributeassignments.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Crie uma atribuição de atributo de usuário em um fluxo de usuário B2C.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|O nome do fluxo de usuário. Esse é um valor obrigatório e imutável após sua criação. O nome será antecedido pelo valor de `B2C_1_` após a criação.|
|userFlowType|Cadeia de caracteres|O [tipo de fluxo de usuário](/azure/active-directory-b2c/user-flow-versions). Os valores com suporte para **userFlowType** são:<br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwner`</li>|
|userFlowTypeVersion|Único|A versão do fluxo de usuário.|

## <a name="relationships"></a>Relações

| Relação       | Tipo  |Descrição|
|:---------------|:--------|:----------|
|identityProviders|Coleção [identityProvider](../resources/identityprovider.md)|Os provedores de identidade incluídos no fluxo de usuário.|
|userAttributeAssignments|Coleção[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) |As atribuições de atributo de usuário incluídas no fluxo do usuário.|

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
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}],
    "userAttributeAssignments": [{"@odate.type": "microsoft.graph.identityUserFlowAttributeAssignment"}]
}
```
