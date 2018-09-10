# <a name="termsandconditionsassignment-resource-type"></a>Tipo de recurso termsAndConditionsAssignment

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar termsAndConditionsAssignments](../api/intune_companyterms_termsandconditionsassignment_list.md)|Coleção [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)|Propriedades de leitura e relações dos objetos [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).|
|[Obter termsAndConditionsAssignment](../api/intune_companyterms_termsandconditionsassignment_get.md)|[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)|Propriedades de leitura e relações do objeto [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).|
|[Criar termsAndConditionsAssignment](../api/intune_companyterms_termsandconditionsassignment_create.md)|[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)|Cria um novo objeto [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).|
|[Excluir termsAndConditionsAssignment](../api/intune_companyterms_termsandconditionsassignment_delete.md)|Nenhum|Exclui um [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).|
|[Atualizar termsAndConditionsAssignment](../api/intune_companyterms_termsandconditionsassignment_update.md)|[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)|Atualiza as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da entidade.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|Destino de atribuição ao qual a política de T&C foi designada.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








