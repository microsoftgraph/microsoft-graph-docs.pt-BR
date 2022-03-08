---
title: Tipo de recurso auditEvent
description: Representa um evento de auditoria para locatários gerenciados Microsoft 365 Lighthouse.
author: vkumar2015
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d0a6097178f160fd305060a4a7d6a289b184228c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338086"
---
# <a name="auditevent-resource-type"></a>Tipo de recurso auditEvent

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um evento de auditoria para locatários gerenciados Microsoft 365 Lighthouse.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar auditEvents](../api/managedtenants-managedtenant-list-auditevents.md)|[coleção microsoft.graph.managedTenants.auditEvent](../resources/managedtenants-auditevent.md)|Obter uma lista dos [objetos auditEvent](../resources/managedtenants-auditevent.md) e suas propriedades.|
|[Obter auditEvent](../api/managedtenants-auditevent-get.md)|[microsoft.graph.managedTenants.auditEvent](../resources/managedtenants-auditevent.md)|Leia as propriedades e as relações de um [objeto auditEvent](../resources/managedtenants-auditevent.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|atividade|Cadeia de caracteres|Uma cadeia de caracteres que representa exclusivamente a operação que ocorreu. Obrigatório. Somente leitura.|
|activityDateTime|DateTimeOffset|O tempo em que a atividade ocorreu. Obrigatório. Somente leitura.|
|activityId|Cadeia de caracteres|O identificador da solicitação de atividade que fez o evento de auditoria. Obrigatório. Somente leitura.|
|category|Cadeia de caracteres|Uma categoria que representa um grupo lógico de atividades. Obrigatório. Somente leitura.|
|httpVerb|Cadeia de caracteres|O verbo HTTP que foi usado ao fazer a solicitação da API. Obrigatório. Somente leitura.|
|id|String|O identificador exclusivo do evento de auditoria. Obrigatório. Somente leitura.|
|initiatedByAppId|String|O identificador do aplicativo que foi usado para fazer a solicitação. Obrigatório. Somente leitura.|
|initiatedByUpn|Cadeia de caracteres|O UPN do usuário que iniciou a atividade. Obrigatório. Somente leitura.|
|initiatedByUserId|String|O identificador do usuário que iniciou a atividade. Obrigatório. Somente leitura.|
|ipAddress|Cadeia de caracteres|O endereço IP de onde a atividade foi iniciada. Pode ser um endereço IPv4 ou IPv6. Obrigatório. Somente leitura.|
|requestBody|String|O corpo da solicitação HTTP bruto. Algumas informações confidenciais podem ser removidas.|
|requestUrl|String|A URL de solicitação HTTP bruta. Obrigatório. Somente leitura.|
|tenantIds|Cadeia de caracteres|A coleção de Azure Active Directory de locatários para os [locatários gerenciados que foram afetados](../resources/managedtenants-tenant.md) por essa alteração. Isso é formatado como uma lista de valores separados por vírgulas. Obrigatório. Somente leitura.|
|tenantNames|String|A coleção de nomes de locatários que foram afetados por essa alteração. Isso é formatado como uma lista de valores separados por vírgulas. Obrigatório. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.auditEvent",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.auditEvent",
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityId": "String",
  "category": "String",
  "httpVerb": "String",
  "id": "String (identifier)",
  "initiatedByAppId": "String",
  "initiatedByUpn": "String",
  "initiatedByUserId": "String",
  "ipAddress": "String",
  "requestBody": "String",
  "requestUrl": "String",
  "tenantIds": "String",
  "tenantNames": "String"
}
```

