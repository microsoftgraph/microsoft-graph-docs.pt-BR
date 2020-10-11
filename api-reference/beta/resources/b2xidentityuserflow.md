---
title: tipo de recurso b2xIdentityUserFlow
description: Representa um fluxo de usuário em um locatário do Azure Active Directory.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 85839539ae78963114ea7a9eaeac49307166a9ff
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406298"
---
# <a name="b2xidentityuserflow-resource-type"></a>tipo de recurso b2xIdentityUserFlow

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um fluxo de usuário em um locatário do Azure Active Directory.

Os fluxos de usuário são usados para habilitar uma experiência de [inscrição de autoatendimento](/azure/active-directory/external-identities/self-service-sign-up-overview) para usuários convidados em um aplicativo. Os fluxos de usuário definem a experiência que o usuário final vê ao se inscrever, inclusive quais [provedores de identidade](/azure/active-directory/external-identities/identity-providers) ele pode usar para autenticação, juntamente com quais atributos são coletados como parte do processo de inscrição.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar fluxos de usuário](../api/identitycontainer-list-b2xuserflows.md)|Coleção b2xIdentityUserFlow|Recupere todos os fluxos de usuário B2X.|
|[Obter fluxo de usuário](../api/b2xidentityuserflow-get.md)|b2xIdentityUserFlow|Recupere as propriedades de um fluxo de usuário B2X.|
|[Criar fluxo de usuário](../api/identitycontainer-post-b2xuserflows.md)|b2xIdentityUserFlow|Crie um novo fluxo de usuário B2X.|
|[Excluir fluxo de usuário](../api/b2xidentityuserflow-delete.md)|Nenhum|Exclua um fluxo de usuário B2X.|
|[Listar os provedores de identidade](../api/b2xidentityuserflow-list-identityproviders.md)|Coleção [identityProvider](../resources/identityProvider.md)|Recupere todos os provedores de identidade em um fluxo de usuário B2X.|
|[Adicionar provedor de identidade](../api/b2xidentityuserflow-post-identityproviders.md)|Nenhum|Adicione um provedor de identidade a um fluxo de usuário B2X.|
|[Remover provedor de identidade](../api/b2xidentityuserflow-delete-identityproviders.md)|Nenhum|Remova um provedor de identidade de um fluxo de usuário B2X.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|O nome do fluxo de usuário. Esse é um valor obrigatório e imutável após sua criação. O nome será antecedido pelo valor de `B2X_1_` após a criação.|
|userFlowType|Cadeia de caracteres|O tipo de fluxo de usuário. Para os fluxos de usuário de inscrição de autoatendimento, o valor só poderá ser `signUpOrSignIn` e não poderá ser modificado após a criação.|
|userFlowTypeVersion|Único|A versão do fluxo de usuário. Para fluxos de usuário B2X, a versão é sempre `1`.|

## <a name="relationships"></a>Relações

| Relação       | Tipo  |Descrição|
|:---------------|:--------|:----------|
|identityProviders|Coleção [identityProvider](../resources/identityprovider.md)|Os provedores de identidade incluídos no fluxo de usuário.|

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
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}]
}
```