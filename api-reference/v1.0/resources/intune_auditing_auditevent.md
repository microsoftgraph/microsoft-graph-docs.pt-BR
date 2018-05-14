# <a name="auditevent-resource-type"></a>Tipo de recurso auditEvent

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma classe que contém as propriedades de Evento de Auditoria.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar auditEvents](../api/intune_auditing_auditevent_list.md)|Conjunto [auditEvent](../resources/intune_auditing_auditevent.md)|Listar propriedades e relações de objetos de [auditEvent](../resources/intune_auditing_auditevent.md).|
|[Obter auditEvent](../api/intune_auditing_auditevent_get.md)|[auditEvent](../resources/intune_auditing_auditevent.md)|Ler propriedades e relações de objetos de[auditEvent](../resources/intune_auditing_auditevent.md).|
|[Criar auditEvent](../api/intune_auditing_auditevent_create.md)|[auditEvent](../resources/intune_auditing_auditevent.md)|Criar um novo objeto de[auditEvent](../resources/intune_auditing_auditevent.md).|
|[Excluir auditEvent](../api/intune_auditing_auditevent_delete.md)|Nenhum|Excluir [auditEvent](../resources/intune_auditing_auditevent.md).|
|[Atualizar auditEvent](../api/intune_auditing_auditevent_update.md)|[auditEvent](../resources/intune_auditing_auditevent.md)|Atualizar as propriedades do objeto de [auditEvent](../resources/intune_auditing_auditevent.md).|
|[Função getAuditCategories](../api/intune_auditing_auditevent_getauditcategories.md)|Conjunto de cadeia de caracteres|Ainda não documentado|
|[Função getAuditActivityTypes](../api/intune_auditing_auditevent_getauditactivitytypes.md)|Conjunto de cadeia de caracteres|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|displayName|Cadeia de caracteres|Nome de exibição do evento.|
|componentName|Cadeia de caracteres|Nome do componente.|
|ator|[auditActor](../resources/intune_auditing_auditactor.md)|Usuários e aplicativos do AAD associados com o evento de auditoria.|
|atividade|Cadeia de caracteres|Nome amigável da atividade.|
|activityDateTime|DateTimeOffset|A hora e data em UTC em que a atividade foi executada.|
|activityType|Cadeia de caracteres|O tipo de atividade que foi executada.|
|activityOperationType|Cadeia de caracteres|O tipo de operação HTTP da atividade.|
|activityResult|Cadeia de caracteres|O resultado da atividade.|
|correlationId|GUID|A ID da solicitação de cliente usada para correlacionar a atividade dentro do sistema.|
|recursos|Conjunto [auditResource](../resources/intune_auditing_auditresource.md)|Recursos em modificação.|
|categoria|Cadeia de caracteres|Categoria de auditoria.|

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
  "correlationId": "<Unknown Primitive Type Edm.Guid>",
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



