# <a name="devicecategory-resource-type"></a>Tipo de recurso deviceCategory

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Categorias de dispositivo fornecem uma maneira de organizar seus dispositivos. Usando categorias de dispositivo, os administradores podem definir suas próprias categorias que fazem sentido para suas empresas. Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceCategories](../api/intune_onboarding_devicecategory_list.md)|Coleção [deviceCategory](../resources/intune_onboarding_devicecategory.md)|Lista propriedades e relações dos objetos [deviceCategory](../resources/intune_onboarding_devicecategory.md).|
|[Obter deviceCategory](../api/intune_onboarding_devicecategory_get.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md)|Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune_onboarding_devicecategory.md).|
|[Criar deviceCategory](../api/intune_onboarding_devicecategory_create.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md)|Cria um novo objeto [deviceCategory](../resources/intune_onboarding_devicecategory.md).|
|[Excluir deviceCategory](../api/intune_onboarding_devicecategory_delete.md)|Nenhuma|Exclui um [deviceCategory](../resources/intune_onboarding_devicecategory.md).|
|[Atualizar deviceCategory](../api/intune_onboarding_devicecategory_update.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md)|Atualiza as propriedades de um objeto [deviceCategory](../resources/intune_onboarding_devicecategory.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo da categoria do dispositivo. Somente leitura.|
|displayName|Cadeia de caracteres|Nome de exibição da categoria de dispositivo.|
|description|Cadeia de caracteres|Descrição opcional da categoria do dispositivo.|

## <a name="relationships"></a>Relações
Nenhuma
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



