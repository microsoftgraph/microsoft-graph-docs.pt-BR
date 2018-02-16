# <a name="user-resource-type"></a>Tipo de recurso de usuário

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ainda não documentado
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar usuários](../api/intune_troubleshooting_user_list.md)|Conjunto [user](../resources/intune_troubleshooting_user.md)|Listar propriedades e relações de objetos de [user](../resources/intune_troubleshooting_user.md).|
|[Obter usuário](../api/intune_troubleshooting_user_get.md)|[user](../resources/intune_troubleshooting_user.md)|Ler propriedades e relações de objetos de [user](../resources/intune_troubleshooting_user.md).|
|[Criar usuário](../api/intune_troubleshooting_user_create.md)|[user](../resources/intune_troubleshooting_user.md)|Criar um novo objeto de [user](../resources/intune_troubleshooting_user.md).|
|[Excluir usuário](../api/intune_troubleshooting_user_delete.md)|Nenhum|Excluir [user](../resources/intune_troubleshooting_user.md).|
|[Atualizar user](../api/intune_troubleshooting_user_update.md)|[user](../resources/intune_troubleshooting_user.md)|Atualizar as propriedades de um objeto de [user](../resources/intune_troubleshooting_user.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do usuário.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceManagementTroubleshootingEvents|Conjunto [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|A lista de eventos de solução de problemas desse usuário.|

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



