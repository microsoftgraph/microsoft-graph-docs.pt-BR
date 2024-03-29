---
title: Tipo de recurso windowsQualityUpdateCatalogItem
description: Windows de item de catálogo de atualização
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1b71b3f0d910b385e60dfb77df488d216b556186
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59029826"
---
# <a name="windowsqualityupdatecatalogitem-resource-type"></a>Tipo de recurso windowsQualityUpdateCatalogItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows de item de catálogo de atualização


Herda de [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsQualityUpdateCatalogItems](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-list.md)|[Coleção windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|Listar propriedades e relações dos [objetos windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|
|[Obter windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-get.md)|[windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|Leia propriedades e relações do [objeto windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|
|[Criar windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-create.md)|[windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|Crie um novo [objeto windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|
|[Excluir windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-delete.md)|Nenhum|Exclui um [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md).|
|[Atualizar windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-update.md)|[windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|Atualize as propriedades de [um objeto windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID do item de catálogo. Herdado [do windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|displayName|Cadeia de caracteres|O nome de exibição do item de catálogo. Herdado [do windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|releaseDateTime|DateTimeOffset|A data em que o item de catálogo foi lançado Herdado de [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|endOfSupportDate|DateTimeOffset|A última data com suporte para um item de catálogo Herdado de [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|kbArticleId|Cadeia de Caracteres|ID do artigo da base de dados de conhecimento|
|classificação|[windowsQualityUpdateClassification](../resources/intune-softwareupdate-windowsqualityupdateclassification.md)|Classificação da atualização de qualidade. Os valores possíveis são: `all`, `security`, `nonSecurity`.|
|isExpeditable|Boolean|Sinalizador indicando se a atualização se qualifica para acelerar|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsQualityUpdateCatalogItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "endOfSupportDate": "String (timestamp)",
  "kbArticleId": "String",
  "classification": "String",
  "isExpeditable": true
}
```



