---
title: tipo de recurso b2xIdentityUserFlow
description: Representa um fluxo de usuário de inscrição de autoatendimento em um locatário do Azure Active Directory.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: 32eea0f34fcfb1b932995e668c672b21c6b7984c
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695340"
---
# <a name="b2xidentityuserflow-resource-type"></a>tipo de recurso b2xIdentityUserFlow

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um fluxo de usuário de inscrição de autoatendimento em um locatário do Azure Active Directory.

Os fluxos de usuário são usados para habilitar uma experiência de [inscrição de autoatendimento](/azure/active-directory/external-identities/self-service-sign-up-overview) para usuários convidados em um aplicativo. Os fluxos de usuário definem a experiência que o usuário final vê ao se inscrever, inclusive quais [provedores de identidade](/azure/active-directory/external-identities/identity-providers) ele pode usar para autenticação, juntamente com quais atributos são coletados como parte do processo de inscrição.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar fluxos de usuário](../api/identitycontainer-list-b2xuserflows.md)|Coleção b2xIdentityUserFlow|Recupere todos os fluxos de usuário B2X.|
|[Obter fluxo de usuário](../api/b2xidentityuserflow-get.md)|b2xIdentityUserFlow|Recupere as propriedades de um fluxo de usuário B2X.|
|[Criar fluxo de usuário](../api/identitycontainer-post-b2xuserflows.md)|b2xIdentityUserFlow|Crie um novo fluxo de usuário B2X.|
|[Excluir fluxo de usuário](../api/b2xidentityuserflow-delete.md)|Nenhum|Exclua um fluxo de usuário B2X.|
|[Listar os provedores de identidade](../api/b2xidentityuserflow-list-userflowidentityproviders.md)|Coleção [identityProvider](../resources/identityproviderbase.md)|Recupere todos os provedores de identidade em um fluxo de usuário B2X.|
|[Adicionar provedor de identidade](../api/b2xidentityuserflow-userflowidentityproviders-update.md)|Nenhum|Adicione um provedor de identidade a um fluxo de usuário B2X.|
|[Remover provedor de identidade](../api/b2xidentityuserflow-delete-userflowidentityproviders.md)|Nenhum|Remova um provedor de identidade de um fluxo de usuário B2X.|
|[Listar os provedores de identidade](../api/b2xidentityuserflow-list-identityproviders.md) (preterido)|Coleção [identityProvider](../resources/identityProvider.md)|Recupere todos os provedores de identidade em um fluxo de usuário B2X.|
|[Adicionar provedor de identidade](../api/b2xidentityuserflow-post-identityproviders.md) (preterido)|Nenhum|Adicione um provedor de identidade a um fluxo de usuário B2X.|
|[Remover provedor de identidade](../api/b2xidentityuserflow-delete-identityproviders.md) (preterido)|Nenhum|Remova um provedor de identidade de um fluxo de usuário B2X.|
|[Listar as atribuições de atributo de usuário](../api/b2xidentityuserflow-list-userattributeassignments.md)|Coleção[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) |Recupere todas as atribuições de atributos do usuário em um fluxo de usuário B2X.|
|[Criar uma tarefa de atributo de usuário](../api/b2xidentityuserflow-post-userattributeassignments.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Crie uma atribuição de atributo de usuário em um fluxo de usuário B2X.|
|[Idiomas da lista](../api/b2xidentityuserflow-list-languages.md)|coleção [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|Recupere todos os idiomas dentro de um fluxo de usuário B2X.|
|[Obtenha a configuração dos conectores de API para o fluxo do usuário](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md)|[userFlowApiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md)| Obtenha a configuração dos conectores de API usados no fluxo do usuário. O parâmetro de consulta $expand não é compatível com este método.|
|[Configurar um conector de API em um fluxo de usuários](../api/b2xidentityuserflow-put-apiConnectorConfiguration.md)|Nenhum| Configure um conector de API para etapas específicas em um fluxo de usuário, atualizando a propriedade [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md).|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|O nome do fluxo de usuário. Esse é um valor obrigatório e imutável após sua criação. O nome será antecedido pelo valor de `B2X_1_` após a criação.|
|userFlowType|userFlowType|O tipo de fluxo de usuário. Para os fluxos de usuário de inscrição de autoatendimento, o valor só poderá ser `signUpOrSignIn` e não poderá ser modificado após a criação.|
|userFlowTypeVersion|Único|A versão do fluxo de usuário. Para fluxos de usuário de inscrição de autoatendimento, a versão é sempre `1`.|
|apiConnectorConfiguration|[userFlowApiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md)|Configuração para habilitar um conector API para uso como parte do fluxo de usuário de inscrição de autoatendimento. Você somente pode obter o valor deste objeto usando [ Obter a userFlowApiConnectorConfiguration ](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md).|

## <a name="relationships"></a>Relações

| Relação       | Tipo  |Descrição|
|:---------------|:--------|:----------|
|userflowIdentityProviders|Coleção [identityProviderBase](../resources/identityproviderbase.md)|Os provedores de identidade incluídos no fluxo de usuários.|
|IdentityProviders (preterido)|Coleção [identityProvider](../resources/identityprovider.md)|Os provedores de identidade incluídos no fluxo de usuário.|
|userAttributeAssignments|Coleção[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) |As atribuições de atributo de usuário incluídas no fluxo do usuário.|
|idiomas|coleção [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|Os idiomas com suporte para personalização dentro do fluxo do usuário. A personalização do idioma é habilitado por padrão no fluxo do usuário de inscrição de autoatendimento. Você não pode criar idiomas personalizados em fluxos de usuário de inscrição de autoatendimento.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow",
  "optionalProperties": [],
  "keyProperty": "id"
} -->

```json
{
    "id": "String (identifier)",
    "userFlowType": "String",
    "userFlowTypeVersion": "Single",
    "userflowIdentityProviders": [{"@odata.type": "microsoft.graph.identityProviderBase"}],
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}],
    "userAttributeAssignments": [{"@odate.type": "microsoft.graph.identityUserFlowAttributeAssignment"}],
    "languages": [{"@odata.type": "microsoft.graph.userFlowLanguageConfiguration"}],
    "apiConnectorConfiguration": {
      "@odata.type": "microsoft.graph.userFlowApiConnectorConfiguration"
    }
}
```
