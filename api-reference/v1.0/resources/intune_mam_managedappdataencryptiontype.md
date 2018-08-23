# <a name="managedappdataencryptiontype-enum-type"></a>tipo de enumeração managedAppDataEncryptionType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useDeviceSettings|0|Os dados do aplicativo são criptografados com base nas configurações padrão do dispositivo.|
|afterDeviceRestart|1|Os dados do aplicativo são criptografados quando o dispositivo for reiniciado.|
|whenDeviceLockedExceptOpenFiles|2|Os dados de aplicativo associados a essa política são criptografados quando o dispositivo for bloqueado, exceto os dados em arquivos que estão abertos|
|whenDeviceLocked|3|Os dados do aplicativo associados a essa política são criptografados quando o dispositivo for bloqueado|



