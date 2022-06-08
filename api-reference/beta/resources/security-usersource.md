---
title: Tipo de recurso userSource
description: O contêiner para a caixa de correio de um usuário e o site do OneDrive for Business.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 45bd3444baa6b3e0aa7c13f6678fd9c2312915b5
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945020"
---
# <a name="usersource-resource-type"></a>Tipo de recurso userSource

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O contêiner para a caixa de correio de um usuário e o site do OneDrive for Business.

Herda de [dataSource](../resources/security-datasource.md).

## <a name="methods"></a>Métodos
Nenhum. 
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou **o userSource**.|
|createdDateTime|DateTimeOffset|A data e a hora em **que o userSource** foi criado|
|displayName|Cadeia de caracteres|O nome de exibição associado à caixa de correio e ao site.|
|email|Cadeia de caracteres|Endereço de email da caixa de correio do usuário.|
|id|Cadeia de caracteres|A ID do **userSource**. Esta não é a ID do grupo real|
|includedSources|Cadeia de caracteres|Especifica quais fontes estão incluídas neste grupo. Os valores possíveis são: `mailbox` e `site`.|
|siteWebUrl|Cadeia de caracteres|A URL do site do OneDrive for Business do usuário. Somente leitura.|
|holdStatus|Cadeia de caracteres|O status de retenção do **userSource**. Os valores possíveis são: `notApplied`, `applied`, `applying`, , `removing``partial`|
### <a name="sourcetype-values"></a>Valores sourceType

Tipos de origem relacionados ao usuário. Inclui caixa de correio e site por padrão.

|Member|Descrição|
|:----|-----------|
|mailbox|Representa uma caixa de correio.|
|site|Representa um site do OneDrive for Business.|

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