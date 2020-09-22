---
title: tipo de recurso continuousAccessEvaluationPolicy
description: A avaliação de acesso contínuo (CAE) ajuda no gerenciamento de sessões de autenticação em tempo real. O CAE permite que os clientes manipulem o acesso a recursos por meio do suporte a eventos de revogação instantânea.
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a3027dea9a6c264b7af0ab805253946ebda8c97
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023422"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a>tipo de recurso continuousAccessEvaluationPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A avaliação de acesso contínuo (CAE) gerencia sessões de autenticação em tempo real. O CAE permite que os clientes manipulem o acesso a recursos por meio do suporte a eventos de revogação instantânea.  Para obter mais informações, consulte a [avaliação de acesso contínuo](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter continuousAccessEvaluationPolicy](../api/continuousaccessevaluationpolicy-get.md)|[continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md)|Ler as propriedades de um objeto [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) .|
|[Atualizar continuousAccessEvaluationPolicy](../api/continuousaccessevaluationpolicy-update.md)|[continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md)|Atualiza as propriedades de um objeto [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) .|
|
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|A avaliação do acesso contínuo bloqueia automaticamente o acesso a recursos e aplicativos, quase em tempo real, quando o acesso de um usuário é removido ou um endereço IP do cliente é alterado. Somente leitura.|
|displayName|String| O valor é sempre ' avaliação de acesso contínuo '. Somente leitura.|
|grupos|Coleção String|A coleção de identificadores de grupo no escopo para avaliação. Todos os grupos estão no escopo quando a coleção está vazia.|
|id|String|Especifica o identificador de um objeto continuousAccessEvaluationPolicy. Somente leitura.|
|isEnabled|Boolean| `true` para indicar se a avaliação de acesso contínuo deve ser executada; caso contrário `false` . |
|usuários|Coleção String|A coleção de identificadores de usuário no escopo para avaliação. Todos os usuários estão no escopo quando a coleção está vazia.|

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
