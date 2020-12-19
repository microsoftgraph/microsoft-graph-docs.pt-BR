---
title: tipo de recurso authenticationEventsPolicy
description: Eventos de autenticação são usados para invocar fluxos de usuário em pontos específicos no fluxo de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cc8789fb0de21980571bdcb5254a7760045e61b0
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720062"
---
# <a name="authenticationeventspolicy-resource-type"></a>tipo de recurso authenticationEventsPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um recurso que especifica os eventos na experiência de autenticação, com cada evento definindo mais detalhadamente os tipos de ouvintes disponíveis que podem ser criados para o evento. Os eventos são inerentes à experiência de autenticação; Este recurso não é configurável pelo usuário.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar ouvintes onSignUpStart](../api/authenticationeventspolicy-list-onsignupstart.md)|coleção [authenticationListener](../resources/authenticationlistener.md)|Obtenha a coleção de recursos authenticationListener com suporte pelo evento onSignupStart.|
|[Criar authenticationListener](../api/authenticationeventspolicy-post-onsignupstart.md)|[authenticationListener](../resources/authenticationlistener.md)|Criar um novo objeto authenticationListener para o evento onSignupStart.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador da política.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|onSignupStart|coleção [authenticationListener](../resources/authenticationlistener.md)|Uma lista de ações aplicáveis a serem executadas na inscrição.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationEventsPolicy",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.authenticationEventsPolicy",
  "id": "String (identifier)"
}
```
