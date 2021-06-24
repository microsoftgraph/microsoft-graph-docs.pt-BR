---
title: Tipo de recurso serviceAnnouncement
description: Um contêiner de nível superior para recursos de comunicações de serviço
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c22cbcd9fd8e67137e649cc099ff7980468c246f
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109069"
---
# <a name="serviceannouncement-resource-type"></a>Tipo de recurso serviceAnnouncement

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um contêiner de nível superior para recursos de comunicações de serviço.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar healthOverviews](../api/serviceannouncement-list-healthoverviews.md)|[Coleção serviceHealth](../resources/servicehealth.md)|Obter os recursos serviceHealth da propriedade de navegação healthOverviews.|
|[Listar problemas](../api/serviceannouncement-list-issues.md)|[Coleção serviceHealthIssue](../resources/servicehealthissue.md)|Obter os recursos serviceHealthIssue da propriedade de navegação de problemas.|
|[Listar mensagens](../api/serviceannouncement-list-messages.md)|[Coleção serviceUpdateMessage](../resources/serviceupdatemessage.md)|Obter os recursos serviceUpdateMessage da propriedade de navegação de mensagens.|

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
|Propriedade|Tipo|Descrição|
|-|-|-|
|messages|Coleção([serviceUpdateMessage](serviceupdatemessage.md))|Uma coleção de mensagens de serviço para locatário. Essa propriedade é uma propriedade de navegação contida, ela é anulada e readonly.|
|healthOverviews|Collection([serviceHealth](servicehealth.md))|Uma coleção de informações de saúde do serviço para locatário. Essa propriedade é uma propriedade de navegação contida, ela é anulada e readonly.|
|issues|Collection([serviceHealthIssue](servicehealthissue.md))|Uma coleção de problemas de serviço para locatário. Essa propriedade é uma propriedade de navegação contida, ela é anulada e readonly.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceAnnouncement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceAnnouncement"
}
```