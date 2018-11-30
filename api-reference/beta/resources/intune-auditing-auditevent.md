---
title: Tipo de recurso auditEvent
description: Uma classe que contém as propriedades de Evento de Auditoria.
ms.openlocfilehash: 1846677ea72dda836f92e0d45d76ea0df0ae74f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039690"
---
# <a name="auditevent-resource-type"></a>Tipo de recurso auditEvent

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma classe que contém as propriedades de Evento de Auditoria.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar auditEvents](../api/intune-auditing-auditevent-list.md)|Conjunto [auditEvent](../resources/intune-auditing-auditevent.md)|Listar propriedades e relações de objetos de [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Obter auditEvent](../api/intune-auditing-auditevent-get.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Ler propriedades e relações de objetos de[auditEvent](../resources/intune-auditing-auditevent.md).|
|[Criar auditEvent](../api/intune-auditing-auditevent-create.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Criar um novo objeto de[auditEvent](../resources/intune-auditing-auditevent.md).|
|[Excluir auditEvent](../api/intune-auditing-auditevent-delete.md)|Nenhum|Excluir [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Atualizar auditEvent](../api/intune-auditing-auditevent-update.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Atualizar as propriedades do objeto de [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Função getAuditCategories](../api/intune-auditing-auditevent-getauditcategories.md)|Conjunto de cadeia de caracteres|Ainda não documentado|
|[Função getAuditActivityTypes](../api/intune-auditing-auditevent-getauditactivitytypes.md)|Conjunto de cadeia de caracteres|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|displayName|Cadeia de caracteres|Nome de exibição do evento.|
|componentName|Cadeia de caracteres|Nome do componente.|
|actor|[auditActor](../resources/intune-auditing-auditactor.md)|Usuários e aplicativos do AAD associados com o evento de auditoria.|
|atividade|Cadeia de caracteres|Nome amigável da atividade.|
|activityDateTime|DateTimeOffset|A hora e data em UTC em que a atividade foi executada.|
|activityType|Cadeia de caracteres|O tipo de atividade que foi executada.|
|activityOperationType|Cadeia de caracteres|O tipo de operação HTTP da atividade.|
|activityResult|Cadeia de caracteres|O resultado da atividade.|
|correlationId|Guid|A ID da solicitação de cliente usada para correlacionar a atividade dentro do sistema.|
|recursos|Coleção [auditResource](../resources/intune-auditing-auditresource.md)|Recursos em modificação.|
|Ferramentas para desenvolvedores|Cadeia de caracteres|Categoria de auditoria.|

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
    "userId": "String"
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





