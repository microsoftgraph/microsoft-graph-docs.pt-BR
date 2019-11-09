---
title: Tipo de recurso auditEvent
description: Uma classe que contém as propriedades de Evento de Auditoria.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 74dba69e146a82cc4b4da8fd7f67c041c5953650
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088165"
---
# <a name="auditevent-resource-type"></a>Tipo de recurso auditEvent

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades de Evento de Auditoria.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar auditEvents](../api/intune-auditing-auditevent-list.md)|Conjunto [auditEvent](../resources/intune-auditing-auditevent.md)|Listar propriedades e relações de objetos de [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Obter auditEvent](../api/intune-auditing-auditevent-get.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Ler propriedades e relações de objetos de[auditEvent](../resources/intune-auditing-auditevent.md).|
|[Criar auditEvent](../api/intune-auditing-auditevent-create.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Criar um novo objeto de[auditEvent](../resources/intune-auditing-auditevent.md).|
|[Excluir auditEvent](../api/intune-auditing-auditevent-delete.md)|Nenhum|Excluir [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Atualizar auditEvent](../api/intune-auditing-auditevent-update.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Atualizar as propriedades do objeto de [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Função getAuditCategories](../api/intune-auditing-auditevent-getauditcategories.md)|String collection|Ainda não documentado|
|[Função getAuditActivityTypes](../api/intune-auditing-auditevent-getauditactivitytypes.md)|Conjunto de cadeia de caracteres|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|displayName|Cadeia de caracteres|Nome de exibição do evento.|
|componentName|String|Nome do componente.|
|actor|[auditActor](../resources/intune-auditing-auditactor.md)|Usuários e aplicativos do AAD associados com o evento de auditoria.|
|atividade|String|Nome amigável da atividade.|
|activityDateTime|DateTimeOffset|A hora e data em UTC em que a atividade foi executada.|
|activityType|String|O tipo de atividade que foi executada.|
|activityOperationType|String|O tipo de operação HTTP da atividade.|
|activityResult|Cadeia de caracteres|O resultado da atividade.|
|correlationId|Guid|A ID da solicitação de cliente usada para correlacionar a atividade dentro do sistema.|
|recursos|Coleção [auditResource](../resources/intune-auditing-auditresource.md)|Recursos em modificação.|
|category|String|Categoria de auditoria.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
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
        "@odata.type": "microsoft.graph.roleScopeTagInfo",
        "displayName": "String",
        "roleScopeTagId": "String"
      }
    ]
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "Guid",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
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



