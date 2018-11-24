# <a name="user-resource-type"></a>Tipo de recurso de usuário

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa um objeto de usuário do Azure Active Directory.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Os usuários da lista](../api/intune_shared_user_list.md) de objetos.|Conjunto [user](../resources/intune_shared_user.md)|Listar propriedades e relações de objetos de [user](../resources/intune_shared_user.md).|
|Objeto [obter do usuário](../api/intune_shared_user_get.md) .|Coleção [user](../resources/intune_shared_user.md)|Leia as propriedades e as relações do objeto [user](../resources/intune_shared_user.md).|
|Objeto de [usuário de criar](../api/intune_shared_user_create.md) .|Coleção [user](../resources/intune_shared_user.md)|Criar um novo objeto de [user](../resources/intune_shared_user.md).|
|[Excluir o usuário](../api/intune_shared_user_delete.md).|Nenhum|Excluir [user](../resources/intune_shared_user.md).|
|Objeto de [usuário de atualização](../api/intune_shared_user_update.md) .|[user](../resources/intune_shared_user.md)|Atualizar as propriedades de um objeto de [user](../resources/intune_shared_user.md).|
|**Gerenciamento de dispositivos**|
|[Ação removeAllDevicesFromManagement](../api/intune_shared_user_removealldevicesfrommanagement.md)|Nenhum|Desativa todos os dispositivos de gerenciamento deste usuário|
|**Gerenciamento de aplicativo móvel (MAM)**|
|[função getManagedAppDiagnosticStatuses](../api/intune_shared_user_getmanagedappdiagnosticstatuses.md)|Conjunto [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md)|Obtém diagnóstico do status de validação para um determinado usuário.|
|[Função getManagedAppPolicies](../api/intune_shared_user_getmanagedapppolicies.md)|Conjunto [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Obtém as restrições de aplicativo para um determinado usuário.|
|[Ação wipeManagedAppRegistrationsByDeviceTag](../api/intune_shared_user_wipemanagedappregistrationsbydevicetag.md)|Nenhum|Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do usuário.|
|**Inclusão**|
|deviceEnrollmentLimit|Int32|O limite do número máximo de dispositivos que o usuário tem permissão para inscrever. Os valores permitidos vão de 5 a 1000.|


## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Gerenciamento de dispositivos**|
|managedDevices|Conjunto [managedDevice](../resources/intune_devices_manageddevice.md)|Os dispositivos gerenciados associados ao usuário.|
|**Gerenciamento de aplicativo móvel (MAM)**|
|managedAppRegistrations|Conjunto [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|Zero ou mais registros de aplicativos gerenciados que pertencem ao usuário.|
|**Solução de problemas**|
|deviceManagementTroubleshootingEvents|Conjunto [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|A lista de eventos de solução de problemas desse usuário.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "@odata.type": "microsoft.graph.user"
}
--> 
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 5
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Resource microsoft.graph.user is defined in multiple files: /api-reference/v1.0/resources/intune_shared_user.md, /api-reference/v1.0/resources/user.md",
  ]
}-->
