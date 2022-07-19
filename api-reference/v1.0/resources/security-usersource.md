---
title: Tipo de recurso userSource
description: O contêiner para a caixa de correio de um usuário e OneDrive for Business site.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 4cd254adcc70a5820dbbec981eb17759f4d034b0
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839042"
---
# <a name="usersource-resource-type"></a>Tipo de recurso userSource

Namespace: microsoft.graph.security



O contêiner para a caixa de correio de um usuário e OneDrive for Business site.

Herda de [dataSource](../resources/security-datasource.md).

## <a name="methods"></a>Métodos
Nenhum. 
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou **o userSource**.|
|createdDateTime|DateTimeOffset|A data e a hora em **que o userSource** foi criado.|
|displayName|Cadeia de caracteres|O nome de exibição associado à caixa de correio e ao site.|
|email|Cadeia de caracteres|Email endereço da caixa de correio do usuário.|
|id|String|A ID do **userSource**. Essa não é a ID do grupo real.|
|includedSources|microsoft.graph.security.sourceType|Especifica quais fontes estão incluídas neste grupo. Os valores possíveis são: `mailbox` e `site`.|
|siteWebUrl|Cadeia de caracteres|A URL do site de OneDrive for Business usuário. Somente leitura.|
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|O status de retenção do **userSource**. Os valores possíveis são: `notApplied`, `applied`, `applying`, `removing`, `partial`.|

### <a name="usersourceholdstatus-values"></a>Valores userSourceHoldStatus

|Nome|Descrição|
|:----|-----------|
|notApplied|O userSource não está em espera (todas as fontes nele não estão em espera).|
|Aplicado|O userSource está em espera (todas as fontes estão em espera).|
|Aplicação|O userSource está aplicando o estado de retenção (operação applyHold disparada).|
|Remover|O userSource está removendo o estado de retenção (operação removeHold disparada).|
|Parcial|O userSource está em estado misto em que algumas fontes estão em espera e outras não estão em espera ou estado de erro.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.userSource",
  "baseType": "microsoft.graph.security.dataSource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.userSource",
  "id": "String (identifier)",
  "displayName": "String",
  "holdStatus": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "email": "String",
  "includedSources": "String",
  "siteWebUrl": "String"
}
```
