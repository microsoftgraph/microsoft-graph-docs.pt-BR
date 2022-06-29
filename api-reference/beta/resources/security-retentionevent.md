---
title: Tipo de recurso retentionEvent
description: Representa um gatilho para rótulos de retenção baseados em eventos em que o início do período de retenção é baseado em quando ocorre um tipo específico de evento.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f44ac532720497888a151776b823884a11782009
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447479"
---
# <a name="retentionevent-resource-type"></a>Tipo de recurso retentionEvent

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um gatilho para rótulos de retenção baseados em eventos em que o início do período de retenção é baseado em quando ocorre um tipo específico de evento.
Para saber mais sobre isso, consulte [Iniciar retenção quando ocorre um evento](/microsoft-365/compliance/event-driven-retention).


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar retentionEvents](../api/security-retentionevent-list.md)|[Coleção microsoft.graph.security.retentionEvent](../resources/security-retentionevent.md)|Obtenha uma lista dos objetos [retentionEvent](../resources/security-retentionevent.md) e suas propriedades.|
|[Criar retentionEvent](../api/security-retentionevent-post.md)|[microsoft.graph.security.retentionEvent](../resources/security-retentionevent.md)|Crie um novo [objeto retentionEvent](../resources/security-retentionevent.md) .|
|[Obter retentionEvent](../api/security-retentionevent-get.md)|[microsoft.graph.security.retentionEvent](../resources/security-retentionevent.md)|Leia as propriedades e as relações de um [objeto retentionEvent](../resources/security-retentionevent.md) .|
|[Excluir retentionEvent](../api/security-retentionevent-delete.md)|Nenhum|Exclua [um objeto retentionEvent](../resources/security-retentionevent.md) .|
|[Listar retentionEventType](../api/security-retentioneventtype-list.md)|[coleção microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Obtenha os recursos retentionEventType da propriedade de navegação exapnd eventType.|
|[Criar retentionEventType](../api/security-retentioneventtype-post.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Adicione eventType adicionando a propriedade odata relevante ao criar um evento.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|O usuário que criou o retentionEvent.|
|createdDateTime|DateTimeOffset|A data em que o retentionEvent foi criado.|
|descrição|Cadeia de caracteres|Informações opcionais sobre o evento.|
|displayName|String|Nome do evento.|
|eventPropagationResult|[microsoft.graph.security.eventPropagationResult](../resources/security-eventpropagationresult.md)|Representa o status de êxito de um evento criado e informações adicionais.|
|eventQueries|[Coleção microsoft.graph.security.eventQueries](../resources/security-eventqueries.md)| Representa a carga de trabalho (SharePoint Online, OneDrive for Business, Exchange Online) e informações de identificação associadas a um evento de retenção.|
|retentionEventStatus|[coleção microsoft.graph.security.retentionEventStatus](../resources/security-retentioneventstatus.md)|Status da propogação de evento para os locais com escopo após a criação do evento.|
|eventTriggerDateTime|DateTimeOffset|Hora opcional em que o evento deve ser disparado.|
|id|Cadeia de caracteres|Representa a ID exclusiva do usuário que criou o retentionEvent. [entidade](/graph/api/resources/entity).|
|lastModifiedBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|O usuário que modificou o retentionEvent pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A hora da data mais recente em que o retentionEvent foi modificado.|
|lastStatusUpdateDateTime|DateTimeOffset|Última vez em que o status do evento foi atualizado.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|retentionEventType|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Especifica o evento que iniciará o período de retenção para rótulos que usam esse tipo de evento quando um evento é criado.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.retentionEvent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "eventQueries": [
    {
      "@odata.type": "microsoft.graph.security.eventQueries"
    }
  ],
  "eventTriggerDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "eventPropagationResults": [
    {
      "@odata.type": "microsoft.graph.security.eventPropagationResult"
    }
  ],
  "eventStatus": {
    "@odata.type": "microsoft.graph.security.retentionEventStatus"
  },
  "lastStatusUpdateDateTime": "String (timestamp)"
}
```