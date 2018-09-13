# <a name="androidmanagedappregistration-resource-type"></a>Tipo de recurso androidManagedAppRegistration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa os detalhes de sincronização de um aplicativo para Android, com recursos de gerenciamento, para um usuário específico.
O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.

Herda de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidManagedAppRegistrations](../api/intune_mam_androidmanagedappregistration_list.md)|Coleção [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md)|Lista propriedades e relações dos objetos [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).|
|[Obter androidManagedAppRegistration](../api/intune_mam_androidmanagedappregistration_get.md)|[androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md)|Propriedades de leitura e relações do objeto [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).|
|[Criar androidManagedAppRegistration](../api/intune_mam_androidmanagedappregistration_create.md)|[androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md)|Crie um novo objeto [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Data e hora de criação. Herdada de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|lastSyncDateTime|DateTimeOffset|Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|applicationVersion|Cadeia de caracteres|Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|managementSdkVersion|Cadeia de caracteres|Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|platformVersion|Cadeia de caracteres|Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|deviceType|Cadeia de caracteres|Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|deviceTag|Cadeia de caracteres|Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo. Sem garantia de indicar aplicativos em todas as condições. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|deviceName|Cadeia de caracteres|Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|flaggedReasons|Coleção [managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md)|Zero ou mais motivos para a sinalização de um registro de aplicativo. Ex: Aplicativo em execução em um dispositivo root. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|userId|Cadeia de caracteres|A ID de usuário à qual este registro de aplicativo pertence. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|appIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|version|Cadeia de caracteres|Versão da entidade. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appliedPolicies|Coleção [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|intendedPolicies|Coleção [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|operations|Coleção [managedAppOperation](../resources/intune_mam_managedappoperation.md)|Zero ou mais operações de longa execução desencadeadas no registro do aplicativo. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedAppRegistration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedAppRegistration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```








