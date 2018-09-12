# <a name="create-androidmanagedappregistration"></a>Criar androidManagedAppRegistration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Cria um novo objeto [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|Token&gt; de portador obrigatório.&lt;|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto androidManagedAppRegistration.

A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedAppRegistration.

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
|flaggedReasons|coleção [managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md)|Zero ou mais motivos pelos quais um registro de aplicativo é sinalizado. Por exemplo, um aplicativo executado em dispositivo desbloqueado herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md). Os valores possíveis são: `none`, `rootedDevice`.|
|userId|Cadeia de caracteres|A ID de usuário à qual este registro de aplicativo pertence. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|appIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|
|versão|Cadeia de caracteres|Versão da entidade. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 753

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value"
}
```








