---
title: Tipo de recurso b2xUserFlows
description: Representa um fluxo de usuário em um locatário do Azure Active Directory.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 989fbb3e003acd4207740a300c1b6f5d0c926e08
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089746"
---
# <a name="b2xuserflows-resource-type"></a>Tipo de recurso b2xUserFlows

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um fluxo de usuário em um locatário do Azure Active Directory.

Os fluxos de usuário são usados para habilitar uma experiência de [inscrição de autoatendimento](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) para usuários convidados em um aplicativo. Os fluxos de usuário definem a experiência que o usuário final vê ao se inscrever, inclusive quais [provedores de identidade](https://docs.microsoft.com/azure/active-directory/external-identities/identity-providers) ele pode usar para autenticação, juntamente com quais atributos são coletados como parte do processo de inscrição.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar fluxos de usuário](../api/b2xuserflows-list.md)|Coleção b2xUserFlow|Recuperar todos os fluxos de usuário.|
|[Obter fluxo de usuário](../api/b2xuserflows-get.md)|b2xUserFlow|Recuperar as propriedades de um fluxo de usuário.|
|[Criar fluxo de usuário](../api/b2xuserflow-post-b2xuserflows.md)|b2xUserFlow|Criar um novo fluxo de usuário.|
|[Excluir fluxo de usuário](../api/b2xuserflows-delete.md)|Nenhum|Excluir um fluxo de usuário.|
|[Listar os provedores de identidade](../api/b2xuserflows-list-identityproviders.md)|Coleção [identityProvider](../resources/identityProvider.md)|Recuperar todos os provedores de identidade em um fluxo de usuário.|
|[Adicionar provedor de identidade](../api/b2xuserflows-update-identityprovider.md)|Nenhum|Adicionar um provedor de identidade a um fluxo de usuário.|
|[Excluir provedor de identidade](../api/b2xuserflows-delete-identityprovider.md)|Nenhum|Excluir um provedor de identidade de um fluxo de usuário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|O nome do fluxo de usuário. Esse é um valor obrigatório e imutável após sua criação. O nome será antecedido pelo valor de `B2X_1_` após a criação.|
|userFlowType|Cadeia de caracteres|O tipo de fluxo de usuário. Para os fluxos de usuário de inscrição de autoatendimento, o valor só poderá ser `signUpOrSignIn` e não poderá ser modificado após a criação.|
|userFlowVersion|Único|A versão do fluxo de usuário. Para fluxos de usuário B2X, a versão é sempre `1`.|

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


