---
title: tipo de recurso b2cIdentityUserFlow
description: Representa um fluxo de usuário em um locatário do Azure Active Directory B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: 8d95fca7096069810c7262eb9a26c91d439c2d55
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957076"
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
|[Atualizar fluxo de usuário](../api/b2cidentityuserflow-update.md)|b2cIdentityUserFlow|Atualizar as propriedades de um fluxo de usuário B2C.|
|[Excluir fluxo de usuário](../api/b2cidentityuserflow-delete.md)|Nenhum|Exclua um fluxo de usuário B2C.|
|[Listar os provedores de identidade](../api/b2cidentityuserflow-list-identityproviders.md)|Coleção [identityProvider](../resources/identityProvider.md)|Recupere todos os provedores de identidade em um fluxo de usuário B2C.|
|[Adicionar provedor de identidade](../api/b2cidentityuserflow-post-identityproviders.md)|Nenhum|Adicione um provedor de identidade a um fluxo de usuário B2C.|
|[Remover provedor de identidade](../api/b2cidentityuserflow-delete-identityproviders.md)|Nenhum|Remova um provedor de identidade de um fluxo de usuário B2C.|
|[Listar as atribuições de atributo de usuário](../api/b2cidentityuserflow-list-userattributeassignments.md)|Coleção[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) |Recupere todas as atribuições de atributos do usuário em um fluxo de usuário B2C.|
|[Criar uma tarefa de atributo de usuário](../api/b2cidentityuserflow-post-userattributeassignments.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Crie uma atribuição de atributo de usuário em um fluxo de usuário B2C.|
|[Idiomas da lista](../api/b2cidentityuserflow-list-languages.md)|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) coleção|Recuperar todos os idiomas no fluxo de usuário do B2C.|
|[Criar idioma](../api/b2cidentityuserflow-put-languages.md)|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|Cria um idioma personalizado em um fluxo de usuário do B2C.|
|[Obtenha a configuração dos conectores de API para o fluxo do usuário](../api/b2cidentityuserflow-get-apiConnectorConfiguration.md)|[userFlowApiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md)| Obtenha a configuração dos conectores de API usados no fluxo do usuário. O parâmetro de consulta $expand não é compatível com este método.|
|[Configurar um conector de API em um fluxo de usuários](../api/b2cidentityuserflow-put-apiConnectorConfiguration.md)|Nenhum| Configure um conector de API para etapas específicas em um fluxo de usuário, atualizando a propriedade [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md).|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|O nome do fluxo de usuário. Esse é um valor obrigatório e imutável após sua criação. O nome será antecedido pelo valor de `B2C_1_` após a criação.|
|userFlowType|userFlowType|O [tipo de fluxo de usuário](/azure/active-directory-b2c/user-flow-versions). Os valores suportados para **userFlowType** são: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`.|
|userFlowTypeVersion|Único|A versão do fluxo de usuário.|
|isLanguageCustomizationEnabled|Booliano|A propriedade que determina se a personalização de idioma é habilitada dentro do fluxo do usuário do B2C. A personalização de idioma não é habilitada por padrão para os fluxos de usuário do B2C.|
|defaultLanguageTag|Cadeia de caracteres|Indica o idioma padrão do b2cIdentityUserFlow que será usado quando nenhuma `ui_locale` marca for especificada na solicitação. Esse campo é [RFC 5646](https://tools.ietf.org/html/rfc5646) compatível.|
|apiConnectorConfiguration|[userFlowApiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md)|Configuração para habilitar um conector de API para uso como parte do fluxo do usuário. Você somente pode obter o valor deste objeto usando [ Obter a userFlowApiConnectorConfiguration ](../api/b2cidentityuserflow-get-apiConnectorConfiguration.md).|

## <a name="relationships"></a>Relações

| Relação       | Tipo  |Descrição|
|:---------------|:--------|:----------|
|identityProviders|Coleção [identityProvider](../resources/identityprovider.md)|Os provedores de identidade incluídos no fluxo de usuário.|
|userAttributeAssignments|Coleção[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) |As atribuições de atributo de usuário incluídas no fluxo do usuário.|
|idiomas|coleção [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|Os idiomas com suporte para personalização dentro do fluxo do usuário. A personalização de idioma não é habilitada por padrão para os fluxos de usuário do B2C.|

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
    "isLanguageCustomizationEnabled": "Boolean",
    "defaultLanguageTag": "String",
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}],
    "userAttributeAssignments": [{"@odate.type": "microsoft.graph.identityUserFlowAttributeAssignment"}],
    "languages": [{"@odata.type": "microsoft.graph.userFlowLanguageConfiguration"}],
    "apiConnectorConfiguration": {
      "@odata.type": "microsoft.graph.userFlowApiConnectorConfiguration"
    }
}
```
