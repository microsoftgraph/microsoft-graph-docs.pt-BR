# <a name="managedappregistration-resource-type"></a>Tipo de recurso managedAppRegistration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.
O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAppRegistrations](../api/intune_mam_managedappregistration_list.md)|Coleção [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|Listar propriedades e relações dos objetos de [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|[Obter managedAppRegistrations](../api/intune_mam_managedappregistration_get.md)|[managedAppRegistration](../resources/intune_mam_managedappregistration.md)|Ler propriedades e relações do objeto [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|[função getUserIdsWithFlaggedAppRegistration](../api/intune_mam_managedappregistration_getuseridswithflaggedappregistration.md)|Coleção String|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Data e hora de criação|
|lastSyncDateTime|DateTimeOffset|Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.|
|applicationVersion|Cadeia de caracteres|Versão do Aplicativo|
|managementSdkVersion|Cadeia de caracteres|Versão do SDK de gerenciamento do aplicativo|
|platformVersion|Cadeia de caracteres|Versão do sistema operacional|
|deviceType|Cadeia de caracteres|Tipo de dispositivo do host|
|deviceTag|Cadeia de caracteres|Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo. Sem garantia de indicar aplicativos em todas as condições.|
|deviceName|Cadeia de caracteres|Nome do dispositivo do host|
|flaggedReasons|coleção enumerada [managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md)|Zero ou mais motivos para a sinalização de um registro de aplicativo. Ex: aplicativo usado em dispositivo modificado|
|userId|Cadeia de caracteres|A ID de usuário à qual este registro de aplicativo pertence.|
|appIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|O identificador do pacote do aplicativo|
|id|Cadeia de caracteres|Chave da entidade.|
|version|Cadeia de caracteres|Versão da entidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appliedPolicies|Coleção [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Zero ou mais políticas já aplicadas ao aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.|
|intendedPolicies|Coleção [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.|
|operations|Coleção [managedAppOperation](../resources/intune_mam_managedappoperation.md)|Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
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
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```
