# <a name="enrollmentconfigurationassignment-resource-type"></a>Tipo de recurso enrollmentConfigurationAssignment

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ainda não documentado
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar enrollmentConfigurationAssignments](../api/intune_onboarding_enrollmentconfigurationassignment_list.md)|Conjunto [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)|Listar propriedades e relações de objetos de [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md).|
|[Obter enrollmentConfigurationAssignment](../api/intune_onboarding_enrollmentconfigurationassignment_get.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)|Ler propriedades e relações de objetos de [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md).|
|[Criar enrollmentConfigurationAssignment](../api/intune_onboarding_enrollmentconfigurationassignment_create.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)|Criar um novo objeto de [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md).|
|[Excluir enrollmentConfigurationAssignment](../api/intune_onboarding_enrollmentconfigurationassignment_delete.md)|Nenhum|Excluir [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md).|
|[Atualizar enrollmentConfigurationAssignment](../api/intune_onboarding_enrollmentconfigurationassignment_update.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)|Atualizar as propriedades de um objeto de [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|Ainda não documentado|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.enrollmentConfigurationAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



