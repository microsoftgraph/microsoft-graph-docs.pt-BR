---
title: Tipo de recurso cloudPcAuditEvent
description: Representa a entidade de evento de auditoria.
author: ecmadao
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 155ecf60bcd160877fe905ef1bd6b328b60bb49d
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507512"
---
# <a name="cloudpcauditevent-resource-type"></a>Tipo de recurso cloudPcAuditEvent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a entidade de evento de auditoria.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar auditEvents](../api/virtualendpoint-list-auditevents.md)|[Coleção cloudPcAuditEvent](../resources/cloudpcauditevent.md)|Listar todos os [objetos cloudPcAuditEvent](../resources/cloudpcauditevent.md) em um locatário.|
|[Obter cloudPcAuditEvent](../api/cloudpcauditevent-get.md)|[cloudPcAuditEvent](../resources/cloudpcauditevent.md)|Leia as propriedades e as relações de um [objeto cloudPcAuditEvent.](../resources/cloudpcauditevent.md)|
|[Função getAuditActivityTypes](../api/cloudpcauditevent-getauditactivitytypes.md)|Conjunto de cadeia de caracteres|Obter tipos de atividade de auditoria.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade de auditoria. Somente leitura.|
|displayName|Cadeia de caracteres|Nome de exibição do evento. Somente leitura.|
|componentName|Cadeia de caracteres|Nome do componente. Somente leitura.|
|actor|[cloudPcAuditActor](../resources/cloudpcauditactor.md)|Usuário e aplicativo do Azure AD associados ao evento de auditoria. Somente leitura.|
|atividade|Cadeia de caracteres|Nome amigável da atividade.Opcional.|
|activityDateTime|DateTimeOffset|A hora e data em UTC em que a atividade foi executada.Somente leitura.|
|activityType|Cadeia de caracteres|O tipo de atividade que foi realizada.Somente leitura.|
|activityOperationType|[cloudPcAuditActivityOperationType](#cloudpcauditactivityoperationtype-values)|O tipo de operação HTTP da atividade. Os valores possíveis  `create` `delete` incluem , e `patch` `other` . Somente leitura.|
|activityResult|[cloudPcAuditActivityResult](#cloudpcauditactivityresult-values)|O resultado da atividade.Somente leitura.|
|correlationId|Cadeia de caracteres|O identificador de solicitação do cliente, usado para correlacionar a atividade no sistema.Somente leitura.|
|recursos|[Coleção cloudPcAuditResource](../resources/cloudpcauditresource.md)|Lista de objetos cloudPcAuditResource.Somente leitura.|
|category|[cloudPcAuditCategory](#cloudpcauditcategory-values)|Categoria de auditoria. Somente leitura.|

### <a name="cloudpcauditactivityoperationtype-values"></a>valores cloudPcAuditActivityOperationType

|Member|Descrição|
|:---|:---|
|create|Criar operação.|
|delete|Excluir operação.|
|patch|Operação patch.|
|other|Outra operação.|

### <a name="cloudpcauditactivityresult-values"></a>valores cloudPcAuditActivityResult

|Member|Descrição|
|:---|:---|
|sucesso|Operação bem-sucedida.|
|clientError|A operação falhou com o erro do cliente.|
|failure|Falha na operação.|
|timeExceeded|A operação falhou com o tempo de tempo.|
|other|Outro resultado.|

### <a name="cloudpcauditcategory-values"></a>valores cloudPcAuditCategory

|Member|Descrição|
|:---|:---|
|cloudPC|Categoria de computador na nuvem.|
|other |Outra categoria.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcAuditEvent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.cloudPcAuditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String",
    "userRoleScopeTags": [
      {
        "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo",
        "displayName": "String",
        "roleScopeTagId": "String"
      }
    ],
    "remoteTenantId": "String",
    "remoteUserId": "String"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.cloudPcAuditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.cloudPcAuditProperty",
          "displayName": "String",
          "oldValue": "String",
          "newValue": "String"
        }
      ],
      "type": "String",
      "resourceId": "String"
    }
  ],
  "category": "String"
}
```
