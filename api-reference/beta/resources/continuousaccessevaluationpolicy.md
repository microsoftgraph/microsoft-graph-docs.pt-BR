---
title: Tipo de recurso continuousAccessEvaluationPolicy
description: A Avaliação de Acesso Contínuo (CAE) ajuda no gerenciamento de sessões de autenticação em tempo real. A CAE permite que os clientes manipularem o acesso a recursos suportando eventos de revogação instantânea.
author: jerrysai
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 299bafe33e4820504180fe64470461d2198b3c13
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559054"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a>Tipo de recurso continuousAccessEvaluationPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A Avaliação de Acesso Contínuo (CAE) gerencia sessões de autenticação em tempo real. A CAE permite que os clientes manipularem o acesso a recursos suportando eventos de revogação instantânea.  Para obter mais informações, consulte a avaliação [de acesso contínuo](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter continuousAccessEvaluationPolicy](../api/continuousaccessevaluationpolicy-get.md)|[continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md)|Leia as propriedades de [um objeto continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)|
|[Atualizar continuousAccessEvaluationPolicy](../api/continuousaccessevaluationpolicy-update.md)|[continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md)|Atualize as propriedades de [um objeto continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)|
|
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|A avaliação de acesso contínuo bloqueia automaticamente o acesso a recursos e aplicativos quase em tempo real quando o acesso de um usuário é removido ou um endereço IP do cliente muda. Somente leitura.|
|displayName|Cadeia de caracteres| O valor é sempre `Continuous Access Evaluation` . Apenas leitura.|
|grupos|Coleção de cadeias de caracteres|A coleção de identificadores de grupo no escopo para avaliação. Todos os grupos estão no escopo quando a coleção está vazia. Somente leitura.|
|id|Cadeia de caracteres|Especifica o identificador de um [objeto continuousAccessEvaluationPolicy.](#continuousaccessevaluationpolicy-resource-type) Somente leitura.|
|isEnabled|Booliano| `true` para indicar se a avaliação de acesso contínuo deve ser realizada; caso `false` contrário. Somente leitura.|
|usuários|Coleção de cadeias de caracteres|A coleção de identificadores de usuário no escopo para avaliação. Todos os usuários estão no escopo quando a coleção está vazia. Apenas leitura.|
|migrar|Boolean| `true` para indicar que as configurações de política de avaliação de acesso contínuo devem ser ou foram migradas para a política de acesso condicional. |
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
  ],
  "migrate": "Boolean"
}
```
