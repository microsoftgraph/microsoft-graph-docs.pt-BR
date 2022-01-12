---
title: Tipo de recurso deploymentAudience
description: O conjunto de recursos updatableAsset aos quais uma implantação pode ser aplicada.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: ab436c0fa9f726528b190fa6fe2f638890447ce4
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61863361"
---
# <a name="deploymentaudience-resource-type"></a>Tipo de recurso deploymentAudience

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O conjunto de [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) aos quais uma [implantação](../resources/windowsupdates-deployment.md) pode ser aplicada.

Se o mesmo **recurso updatableAsset** estiver  incluído nas exclusões e relações de membros, a implantação não se aplicará a ele. 

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar membros](../api/windowsupdates-deploymentaudience-list-members.md)|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Listar membros da [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).|
|[Exclusões de lista](../api/windowsupdates-deploymentaudience-list-exclusions.md)|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Listar exclusões da [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).|
|[Atualizar membros e exclusões](../api/windowsupdates-deploymentaudience-updateaudience.md)|Nenhum|Adicionar ou remover membros e exclusões.|
|[Atualizar membros e exclusões (por ID)](../api/windowsupdates-deploymentaudience-updateaudiencebyid.md)|Nenhum|Adicione ou remova membros e exclusões do mesmo tipo.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo para o público de implantação. Devolvido por padrão. Chave. Não anulável. Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|exclusões|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Especifica os ativos a ser excluídos da audiência.|
|members|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Especifica os ativos a ser incluídos na audiência.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentAudience",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentAudience",
  "id": "String (identifier)"
}
```

