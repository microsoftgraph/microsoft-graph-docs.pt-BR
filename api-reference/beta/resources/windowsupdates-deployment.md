---
title: tipo de recurso de implantação
description: Representa a implantação de conteúdo para um conjunto de dispositivos.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: d4d34481b6a1d99d7c2a48b3becd7b8def764924
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61841939"
---
# <a name="deployment-resource-type"></a>tipo de recurso de implantação

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a implantação de conteúdo para um conjunto de dispositivos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar implantações](../api/windowsupdates-updates-list-deployments.md)|[coleção microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)|Obter uma lista dos objetos [de implantação](../resources/windowsupdates-deployment.md) e suas propriedades.|
|[Criar implantação](../api/windowsupdates-updates-post-deployments.md)|[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)|Crie um novo [objeto de implantação.](../resources/windowsupdates-deployment.md)|
|[Obter implantação](../api/windowsupdates-deployment-get.md)|[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)|Leia as propriedades e as relações de um [objeto de](../resources/windowsupdates-deployment.md) implantação.|
|[Atualizar implantação](../api/windowsupdates-deployment-update.md)|[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)|Atualize as propriedades de um [objeto de](../resources/windowsupdates-deployment.md) implantação.|
|[Excluir implantação](../api/windowsupdates-deployment-delete.md)|Nenhum|Exclui um [objeto de implantação.](../resources/windowsupdates-deployment.md)|
|[Listar membros da audiência](../api/windowsupdates-deploymentaudience-list-members.md)|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Listar membros da audiência de implantação.|
|[Listar exclusões de audiência](../api/windowsupdates-deploymentaudience-list-exclusions.md)|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Listar exclusões da audiência de implantação.|
|[Atualizar membros da audiência e exclusões](../api/windowsupdates-deploymentaudience-updateaudience.md)|Nenhum|Adicionar ou remover membros e exclusões da audiência de implantação.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|content|[microsoft.graph.windowsUpdates.deployableContent](../resources/windowsupdates-deployablecontent.md)|Especifica qual conteúdo implantar. Não é possível mudar. Retornado por padrão.|
|createdDateTime|DateTimeOffset|A data e a hora em que a implantação foi criada. Retornado por padrão. Somente leitura.|
|id|String|O identificador exclusivo da implantação. Devolvido por padrão. Chave. Não anulável. Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a implantação foi modificada pela última vez. Retornado por padrão. Somente leitura.|
|settings|[microsoft.graph.windowsUpdates.deploymentSettings](../resources/windowsupdates-deploymentsettings.md)|Configurações especificado na implantação específica que rege como implantar **conteúdo**. Retornado por padrão.|
|state|[microsoft.graph.windowsUpdates.deploymentState](../resources/windowsupdates-deploymentstate.md)|Status de execução da implantação. Retornado por padrão.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|audience|[microsoft.graph.windowsUpdates.deploymentAudience](../resources/windowsupdates-deploymentaudience.md)|Especifica a audiência para a qual o conteúdo é implantado.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.deployment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "id": "String (identifier)",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
  },
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.deployableContent"
  },
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

