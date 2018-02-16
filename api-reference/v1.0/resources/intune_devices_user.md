# <a name="user-resource-type"></a>Tipo de recurso de usuário

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ainda não documentado
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar usuários](../api/intune_devices_user_list.md)|Conjunto [user](../resources/intune_devices_user.md)|Listar propriedades e relações de objetos de [user](../resources/intune_devices_user.md).|
|[Obter usuário](../api/intune_devices_user_get.md)|[user](../resources/intune_devices_user.md)|Ler propriedades e relações de objetos de [user](../resources/intune_devices_user.md).|
|[Criar usuário](../api/intune_devices_user_create.md)|[user](../resources/intune_devices_user.md)|Criar um novo objeto de [user](../resources/intune_devices_user.md).|
|[Excluir usuário](../api/intune_devices_user_delete.md)|Nenhum|Excluir [user](../resources/intune_devices_user.md).|
|[Atualizar user](../api/intune_devices_user_update.md)|[user](../resources/intune_devices_user.md)|Atualizar as propriedades de um objeto de [user](../resources/intune_devices_user.md).|
|[Ação removeAllDevicesFromManagement](../api/intune_devices_user_removealldevicesfrommanagement.md)|Nenhum|Desativa todos os dispositivos de gerenciamento deste usuário|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do usuário.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedDevices|Conjunto [managedDevice](../resources/intune_devices_manageddevice.md)|Os dispositivos gerenciados associados ao usuário.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



