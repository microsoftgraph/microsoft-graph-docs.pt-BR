---
title: Tipo de recurso cloudPcAuditEvent
description: Representa a entidade de evento de auditoria.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: a863ea4128b7383c70bd14f025fcc5ce116dda25
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211193"
---
# <a name="cloudpcauditevent-resource-type"></a>Tipo de recurso cloudPcAuditEvent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a entidade de evento de auditoria.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar auditEvents](../api/virtualendpoint-list-auditevents.md)|[Coleção cloudPcAuditEvent](../resources/cloudpcauditevent.md)|Listar todos os [objetos cloudPcAuditEvent](../resources/cloudpcauditevent.md) em um locatário.|
|[Obter cloudPcAuditEvent](../api/cloudpcauditevent-get.md)|[cloudPcAuditEvent](../resources/cloudpcauditevent.md)|Leia as propriedades e as relações de um [objeto cloudPcAuditEvent.](../resources/cloudpcauditevent.md)|
|[Função getAuditActivityTypes](../api/cloudpcauditevent-getauditactivitytypes.md)|Conjunto de cadeia de caracteres|Obter tipos de atividade de auditoria.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade de auditoria. Somente leitura.|
|displayName|String|Nome de exibição do evento. Só leitura.|
|componentName|Cadeia de caracteres|Nome do componente. Somente leitura.|
|actor|[cloudPcAuditActor](../resources/cloudpcauditactor.md)|Usuário e aplicativo do Azure AD associados ao evento de auditoria. Só leitura.|
|atividade|Cadeia de caracteres|Nome amigável da atividade.Opcional.|
|activityDateTime|DateTimeOffset|A hora e data em UTC em que a atividade foi executada.Só leitura.|
|activityType|Cadeia de caracteres|O tipo de atividade que foi realizada.Só leitura.|
|activityOperationType|[cloudPcAuditActivityOperationType](#cloudpcauditactivityoperationtype-values)|O tipo de operação HTTP da atividade. Os valores possíveis  `create` `delete` incluem , e `patch` `other` . Só leitura.|
|activityResult|[cloudPcAuditActivityResult](#cloudpcauditactivityresult-values)|O resultado da atividade.Só leitura.|
|correlationId|Cadeia de caracteres|O identificador de solicitação do cliente, usado para correlacionar a atividade no sistema.Só leitura.|
|recursos|[Coleção cloudPcAuditResource](../resources/cloudpcauditresource.md)|Lista de objetos cloudPcAuditResource.Só leitura.|
|category|[cloudPcAuditCategory](#cloudpcauditcategory-values)|Categoria de auditoria. Só leitura.|

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
