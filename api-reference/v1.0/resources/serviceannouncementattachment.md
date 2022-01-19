---
title: Tipo de recurso serviceAnnouncementAttachment
description: Representa um anexo associado a um objeto serviceUpdateMessage.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 8b00cacb19784f34700089d59de22183b8f6e98a
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072730"
---
# <a name="serviceannouncementattachment-resource-type"></a>Tipo de recurso serviceAnnouncementAttachment

Namespace: microsoft.graph

Representa um anexo associado a um [objeto serviceUpdateMessage.](../resources/serviceupdatemessage.md)

Herda do [anexo](../resources/attachment.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter serviceAnnouncementAttachment](../api/serviceannouncementattachment-get.md)|[serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md)|Leia as propriedades e as relações de um [objeto serviceAnnouncementAttachment.](../resources/serviceannouncementattachment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|conteúdo|Fluxo|O conteúdo do anexo.|
|contentType|String|O tipo de conteúdo do anexo.|
|id|String|A ID do anexo. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Data e hora em que o anexo foi modificado pela última vez.|
|name|Cadeia de caracteres|O nome do anexo.|
|size|Int32|O tamanho do anexo em bytes.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceAnnouncementAttachment",
  "baseType": "microsoft.graph.attachment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceAnnouncementAttachment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "contentType": "String",
  "size": "Integer",
  "isInline": "Boolean",
  "content": "Stream"
}
```
