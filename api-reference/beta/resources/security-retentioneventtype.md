---
title: Tipo de recurso retentionEventType
description: Representa um único grupo para o mesmo tipo de eventos de retenção. Um tipo de evento é uma desinsripção genérica para eventos semelhantes que podem ser usados com qualquer rótulo com retenção baseada em evento.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 38b9ee622663d249c5f6c117b376767eb29ae232
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447519"
---
# <a name="retentioneventtype-resource-type"></a>Tipo de recurso retentionEventType

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um único grupo para o mesmo tipo de eventos de retenção.

Quando um [evento de retenção](../resources/security-retentionevent.md) é criado, ele é associado a um tipo de evento específico que, por sua vez, está associado a um [rótulo de retenção](../resources/security-retentionlabel.md). Somente o conteúdo com esse rótulo de retenção aplicado será retido pelo período de retenção especificado.
Para obter detalhes, consulte [Iniciar retenção quando ocorre um evento](/microsoft-365/compliance/event-driven-retention).


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar retentionEventTypes](../api/security-retentioneventtype-list.md)|[coleção microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Obtenha uma lista dos [objetos retentionEventType](../resources/security-retentioneventtype.md) e suas propriedades.|
|[Criar retentionEventType](../api/security-retentioneventtype-post.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Crie um novo [objeto retentionEventType](../resources/security-retentioneventtype.md) .|
|[Obter retentionEventType](../api/security-retentioneventtype-get.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Leia as propriedades e as relações de um [objeto retentionEventType](../resources/security-retentioneventtype.md) .|
|[Atualizar retentionEventType](../api/security-retentioneventtype-update.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Atualize as propriedades de [um objeto retentionEventType](../resources/security-retentioneventtype.md) .|
|[Excluir retentionEventType](../api/security-retentioneventtype-delete.md)|Nenhum|[Exclua um objeto retentionEventType](../resources/security-retentioneventtype.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|O usuário que criou o retentionEventType.|
|createdDateTime|DateTimeOffset|A data em que o retentionEventType foi criado.|
|description|Cadeia de caracteres|Informações opcionais sobre o tipo de evento.|
|displayName|Cadeia de caracteres|Nome do tipo de evento.|
|id|Cadeia de caracteres|Representa a ID exclusiva do usuário que criou o retentionEventType. [entidade](/graph/api/resources/entity).|
|lastModifiedBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|O usuário que modificou o retentionEventType pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A data mais recente em que o retentionEventType foi modificado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.retentionEventType",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionEventType",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```

