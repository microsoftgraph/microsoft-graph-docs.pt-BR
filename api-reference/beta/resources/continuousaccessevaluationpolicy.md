---
title: Tipo de recurso continuousAccessEvaluationPolicy
description: A Avaliação de Acesso Contínuo (CAE) ajuda no gerenciamento de sessões de autenticação em tempo real. A CAE permite que os clientes manipularem o acesso a recursos suportando eventos de revogação instantânea.
author: jerrysai
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 58c4f913c8a5fc3b4f7c1c129c7126437035cbe7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444260"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a>Tipo de recurso continuousAccessEvaluationPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A Avaliação de Acesso Contínuo (CAE) gerencia sessões de autenticação em tempo real. A CAE permite que os clientes manipularem o acesso a recursos suportando eventos de revogação instantânea.  Para obter mais informações, consulte a avaliação [de acesso contínuo](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter continuousAccessEvaluationPolicy](../api/continuousaccessevaluationpolicy-get.md)|[continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md)|Leia as propriedades de [um objeto continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)|
|[Atualizar continuousAccessEvaluationPolicy](../api/continuousaccessevaluationpolicy-update.md)|[continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md)|Atualize as propriedades de [um objeto continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)|
|
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|A avaliação de acesso contínuo bloqueia automaticamente o acesso a recursos e aplicativos quase em tempo real quando o acesso de um usuário é removido ou um endereço IP do cliente muda. Somente leitura.|
|displayName|String| O valor é sempre "Avaliação de Acesso Contínuo". Somente leitura.|
|grupos|Coleção de cadeias de caracteres|A coleção de identificadores de grupo no escopo para avaliação. Todos os grupos estão no escopo quando a coleção está vazia.|
|id|String|Especifica o identificador de um objeto continuousAccessEvaluationPolicy. Somente leitura.|
|isEnabled|Booliano| `true` para indicar se a avaliação de acesso contínuo deve ser realizada; caso `false` contrário. |
|usuários|Coleção de cadeias de caracteres|A coleção de identificadores de usuário no escopo para avaliação. Todos os usuários estão no escopo quando a coleção está vazia.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.continuousAccessEvaluationPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "isEnabled": "Boolean",
  "users": [
    "String"
  ],
  "groups": [
    "String"
  ]
}
```
