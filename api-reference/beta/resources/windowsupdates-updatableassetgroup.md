---
title: Tipo de recurso updatableAssetGroup
description: Um grupo de recursos do azureADDevice que podem receber atualizações.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a3aca42b69a906f167393cfd284d6756b3c4bb52
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067233"
---
# <a name="updatableassetgroup-resource-type"></a>Tipo de recurso updatableAssetGroup

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um grupo de [recursos do azureADDevice](../resources/windowsupdates-azureaddevice.md) que podem receber atualizações.

Os membros são do tipo de [recurso azureADDevice.](../resources/windowsupdates-azureADDevice.md) Um **recurso updatableAssetGroup** não pode ser membro de outro **updatableAssetGroup**.

Herda de [updatableAsset](../resources/windowsupdates-updatableasset.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar recursos updatableAssetGroup](../api/windowsupdates-updates-list-updatableassets-updatableassetgroup.md)|[coleção microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)|Obter uma lista dos objetos [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) e suas propriedades.|
|[Criar updatableAssetGroup](../api/windowsupdates-updates-post-updatableassets-updatableassetgroup.md)|[microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)|Crie um novo [objeto updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)|
|[Obter updatableAssetGroup](../api/windowsupdates-updatableassetgroup-get.md)|[microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)|Leia as propriedades e as relações de um [objeto updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)|
|[Excluir updatableAssetGroup](../api/windowsupdates-updatableassetgroup-delete.md)|Nenhum|Exclui um [objeto updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)|
|[Adicionar membros](../api/windowsupdates-updatableassetgroup-addmembers.md)|Nenhum|Adicionar membros a [um updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).|
|[Adicionar membros (por ID)](../api/windowsupdates-updatableassetgroup-addmembers.md)|Nenhum|Adicionar membros a [um updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).|
|[Remover membros](../api/windowsupdates-updatableassetgroup-removemembers.md)|Nenhum|Remover membros de [um updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).|
|[Remover membros (por ID)](../api/windowsupdates-updatableassetgroup-removemembers.md)|Nenhum|Remover membros de [um updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).|
|[Listar membros](../api/windowsupdates-updatableassetgroup-list-members.md)|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Obter os [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) da propriedade de navegação membros.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Um identificador para o grupo. Chave. Não anulável. Somente leitura. Retornado por padrão. Herdado [de updatableAsset](../resources/windowsupdates-updatableasset.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|membros|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Membros do grupo. Somente leitura.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetGroup",
  "baseType": "microsoft.graph.windowsUpdates.updatableAsset",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
  "id": "String (identifier)"
}
```

