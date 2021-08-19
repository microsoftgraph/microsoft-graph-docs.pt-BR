---
title: Tipo de recurso windowsFeatureUpdateCatalogItem
description: Windows de item de catálogo de atualização
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 44ae53e633497399cba7a64f89f1fa49bf7635a18ca986ad9839b9c140ba60a8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54224338"
---
# <a name="windowsfeatureupdatecatalogitem-resource-type"></a>Tipo de recurso windowsFeatureUpdateCatalogItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows de item de catálogo de atualização


Herda de [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsFeatureUpdateCatalogItems](../api/intune-softwareupdate-windowsfeatureupdatecatalogitem-list.md)|[Coleção windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|Listar propriedades e relações dos [objetos windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|
|[Obter windowsFeatureUpdateCatalogItem](../api/intune-softwareupdate-windowsfeatureupdatecatalogitem-get.md)|[windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|Ler propriedades e relações do [objeto windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|
|[Criar windowsFeatureUpdateCatalogItem](../api/intune-softwareupdate-windowsfeatureupdatecatalogitem-create.md)|[windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|Crie um novo [objeto windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|
|[Excluir windowsFeatureUpdateCatalogItem](../api/intune-softwareupdate-windowsfeatureupdatecatalogitem-delete.md)|Nenhum|Exclui um [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md).|
|[Atualizar windowsFeatureUpdateCatalogItem](../api/intune-softwareupdate-windowsfeatureupdatecatalogitem-update.md)|[windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|Atualize as propriedades de um [objeto windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do item de catálogo. Herdado [do windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|displayName|Cadeia de caracteres|O nome de exibição do item de catálogo. Herdado [do windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|releaseDateTime|DateTimeOffset|A data em que o item de catálogo foi lançado Herdado de [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|endOfSupportDate|DateTimeOffset|A última data com suporte para um item de catálogo Herdado de [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|versão|String|A versão de atualização de recursos|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsFeatureUpdateCatalogItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "endOfSupportDate": "String (timestamp)",
  "version": "String"
}
```




