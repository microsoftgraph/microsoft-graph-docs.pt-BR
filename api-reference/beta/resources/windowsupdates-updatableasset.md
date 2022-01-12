---
title: Tipo de recurso updatableAsset
description: Representa um ativo que pode receber atualizações.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: af8759504e5b79a28686a9070de23c522b9eb0e3
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61859964"
---
# <a name="updatableasset-resource-type"></a>Tipo de recurso updatableAsset

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um ativo que pode receber atualizações.

Todos os ativos atualizáveis existem como um dos seguintes tipos derivados: [azureADDevice](../resources/windowsupdates-azureaddevice.md) e [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).

Tipo base de [azureADDevice](../resources/windowsupdates-azureaddevice.md) e [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).

Esse é um tipo abstrato.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar recursos updatableAsset](../api/windowsupdates-updates-list-updatableassets.md)|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Obter uma lista dos objetos [updatableAsset](../resources/windowsupdates-updatableasset.md) e suas propriedades.|
|[Criar updatableAssetGroup](../api/windowsupdates-updates-post-updatableassets-updatableassetgroup.md)|[microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)|Crie um novo [objeto updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)|
|[Obter updatableAsset](../api/windowsupdates-updatableasset-get.md)|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Leia as propriedades e as relações de um [objeto updatableAsset.](../resources/windowsupdates-updatableasset.md)|
|[Excluir updatableAsset](../api/windowsupdates-updatableasset-delete.md)|Nenhum|[Exclua um objeto updatableAsset.](../resources/windowsupdates-updatableasset.md)|
|[Registrar ativo no gerenciamento](../api/windowsupdates-updatableasset-enrollassets.md)|Nenhum|Registrar [updatableAssets](../resources/windowsupdates-updatableasset.md) no gerenciamento de atualizações pelo serviço de implantação.|
|[Registrar ativo no gerenciamento (por ID)](../api/windowsupdates-updatableasset-enrollassetsbyid.md)|Nenhum|Registrar [updatableAssets](../resources/windowsupdates-updatableasset.md) do mesmo tipo no gerenciamento de atualizações pelo serviço de implantação.|
|[Desemarro o ativo do gerenciamento](../api/windowsupdates-updatableasset-unenrollassets.md)|Nenhum|Unenroll [updatableAssets](../resources/windowsupdates-updatableasset.md) from update management by the deployment service.|
|[Desemroll asset from management (by ID)](../api/windowsupdates-updatableasset-unenrollassetsbyid.md)|Nenhum|Unenroll [updatableAssets](../resources/windowsupdates-updatableasset.md) of the same type from update management by the deployment service.|
|[Adicionar membros ao grupo](../api/windowsupdates-updatableassetgroup-addmembers.md)|Nenhum|Adicionar membros a [um updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).|
|[Adicionar membros ao grupo (por ID)](../api/windowsupdates-updatableassetgroup-addmembersbyid.md)|Nenhum|Adicione membros do mesmo tipo a um [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).|
|[Remover membros do grupo](../api/windowsupdates-updatableassetgroup-removemembers.md)|Nenhum|Remover membros de [um updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).|
|[Remover membros do grupo (por ID)](../api/windowsupdates-updatableassetgroup-removemembersbyid.md)|Nenhum|Remover membros do mesmo tipo de um [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Um identificador para o ativo. Chave. Não anulável. Somente leitura. Devolvido por padrão.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAsset",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
  "id": "String (identifier)"
}
```

