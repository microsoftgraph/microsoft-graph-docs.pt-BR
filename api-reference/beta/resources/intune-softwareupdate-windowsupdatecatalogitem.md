---
title: Tipo de recurso windowsUpdateCatalogItem
description: Windows de item de catálogo de atualização
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c3aff1578b02e7cd3c6a06fda142501fd96c2f30
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039032"
---
# <a name="windowsupdatecatalogitem-resource-type"></a>Tipo de recurso windowsUpdateCatalogItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows de item de catálogo de atualização

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsUpdateCatalogItems](../api/intune-softwareupdate-windowsupdatecatalogitem-list.md)|[Coleção windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|Listar propriedades e relações dos [objetos windowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|[Obter windowsUpdateCatalogItem](../api/intune-softwareupdate-windowsupdatecatalogitem-get.md)|[windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|Ler propriedades e relações do [objeto windowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do item de catálogo.|
|displayName|Cadeia de caracteres|O nome de exibição do item de catálogo.|
|releaseDateTime|DateTimeOffset|A data em que o item de catálogo foi lançado|
|endOfSupportDate|DateTimeOffset|A última data com suporte para um item de catálogo|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateCatalogItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateCatalogItem",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "endOfSupportDate": "String (timestamp)"
}
```



