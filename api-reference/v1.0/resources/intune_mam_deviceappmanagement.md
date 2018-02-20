# <a name="deviceappmanagement-resource-type"></a>Tipo de recurso deviceAppManagement

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade singleton de gerenciamento de aplicativos do dispositivo.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceAppManagement](../api/intune_mam_deviceappmanagement_get.md)|[deviceAppManagement](../resources/intune_mam_deviceappmanagement.md)|Propriedades de leitura e relações do objeto [deviceAppManagement](../resources/intune_mam_deviceappmanagement.md).|
|[Atualizar deviceAppManagement](../api/intune_mam_deviceappmanagement_update.md)|[deviceAppManagement](../resources/intune_mam_deviceappmanagement.md)|Atualiza as propriedades de um objeto [deviceAppManagement](../resources/intune_mam_deviceappmanagement.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedAppPolicies|Coleção [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Políticas de aplicativos gerenciados.|
|iosManagedAppProtections|Coleção [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md)|Políticas de aplicativos gerenciados para iOS.|
|androidManagedAppProtections|Coleção [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md)|Políticas de aplicativos gerenciados para Android.|
|defaultManagedAppProtections|Coleção [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md)|Políticas de aplicativos gerenciados padrão.|
|targetedManagedAppConfigurations|Coleção [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)|Configurações de aplicativos gerenciados direcionadas.|
|mdmWindowsInformationProtectionPolicies|Coleção [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md)|Proteção de informações do Windows para aplicativos em execução em dispositivos que estão registrados no MDM.|
|windowsInformationProtectionPolicies|Coleção [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)|Proteção de informações do Windows para aplicativos em execução em dispositivos que não estão registrados no MDM.|
|managedAppRegistrations|Coleção [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|Os registros de aplicativos gerenciados.|
|managedAppStatuses|Coleção [managedAppStatus](../resources/intune_mam_managedappstatus.md)|Os status de aplicativos gerenciados.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



