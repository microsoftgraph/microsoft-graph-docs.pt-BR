---
title: Tipo de recurso accessReviewPolicy
description: A política de revisões do Access é um singleton que permite que as organizações gerenciem a política de revisão de acesso no nível do diretório.
author: kafen
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 02940987682d84aa3fc3dbb076c998abfe24bf8e
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067811"
---
# <a name="accessreviewpolicy-resource-type"></a>Tipo de recurso accessReviewPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A política de revisão do Access é um singleton que permite que os administradores gerenciem políticas de revisão de acesso no nível do diretório. Por exemplo, os administradores podem usar a política de revisão de acesso para habilitar e desabilitar a capacidade dos proprietários do grupo de criar avaliações de acesso nos grupos que eles têm.


Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter accessReviewPolicy](../api/accessreviewpolicy-get.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|Leia as propriedades e as relações de um [objeto accessReviewPolicy.](../resources/accessreviewpolicy.md)|
|[Atualizar accessReviewPolicy](../api/accessreviewpolicy-update.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|Atualize as propriedades de [um objeto accessReviewPolicy.](../resources/accessreviewpolicy.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|Descrição dessa política. Somente leitura.|
|displayName|Cadeia de caracteres|Nome de exibição para esta política. Somente leitura.|
|isGroupOwnerManagementEnabled|Boolean|Se `true` , os proprietários do grupo podem criar e gerenciar avaliações de acesso nos grupos que eles próprios têm.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewPolicy",
  "displayName": "Access Review Policy",
  "description": "Policy contains directory-level access review settings.",
  "isGroupOwnerManagementEnabled": false
}
```
