# <a name="androidforworkenrollmentprofile-resource-type"></a>Tipo de recurso androidForWorkEnrollmentProfile

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Perfil de registro usado para registrar dispositivos COSU usando o Gerenciamento de Nuvem do Google.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidForWorkEnrollmentProfiles](../api/intune_androidforwork_androidforworkenrollmentprofile_list.md)|Coleção [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|Lista propriedades e relações dos objetos [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).|
|[Obter androidForWorkEnrollmentProfile](../api/intune_androidforwork_androidforworkenrollmentprofile_get.md)|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|Propriedades de leitura e relações do objeto [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).|
|[Criar androidForWorkEnrollmentProfile](../api/intune_androidforwork_androidforworkenrollmentprofile_create.md)|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|Cria um novo objeto [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).|
|[Excluir androidForWorkEnrollmentProfile](../api/intune_androidforwork_androidforworkenrollmentprofile_delete.md)|Nenhuma|Exclui um [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).|
|[Atualizar androidForWorkEnrollmentProfile](../api/intune_androidforwork_androidforworkenrollmentprofile_update.md)|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|Atualiza as propriedades de um objeto [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).|
|[Ação revokeToken](../api/intune_androidforwork_androidforworkenrollmentprofile_revoketoken.md)|Nenhuma|Ainda não documentado|
|[Ação createToken](../api/intune_androidforwork_androidforworkenrollmentprofile_createtoken.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accountId|Cadeia de caracteres|GUID de locatário ao qual o perfil de registro pertence.|
|id|Cadeia de caracteres|GUID exclusivo do perfil de registro.|
|name|Cadeia de caracteres|(Preterido) Nome de exibição do perfil de registro.|
|displayName|Cadeia de caracteres|Nome de exibição do perfil de registro.|
|description|Cadeia de caracteres|Descrição do perfil de registro.|
|createdDateTime|DateTimeOffset|Data e hora de criação do perfil de registro.|
|modifiedDateTime|DateTimeOffset|(Preterido) Data e hora da última modificação do perfil de registro.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação do perfil de registro.|
|tokenValue|Cadeia de caracteres|Valor do token mais recentemente criado para este perfil de registro.|
|tokenExpirationDateTime|DateTimeOffset|Data e hora em que o token mais recentemente criado expirará.|
|totalEnrollmentCount|Int32|(Preterido) Número total de dispositivos Android que foram registrados usando esse perfil de registro.|
|enrolledDeviceCount|Int32|Número total de dispositivos Android que foram registrados usando esse perfil de registro.|
|qrCode|Cadeia de caracteres|(Preterido) Cadeia de caracteres usada para gerar um código QR para o token.|
|qrCodeContent|Cadeia de caracteres|Cadeia de caracteres usada para gerar um código QR para o token.|
|qrCodeImage|[mimeContent](../resources/intune_androidforwork_mimecontent.md)|Cadeia de caracteres usada para gerar um código QR para o token.|

## <a name="relationships"></a>Relações
Nenhuma
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "name": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
  "tokenExpirationDateTime": "String (timestamp)",
  "totalEnrollmentCount": 1024,
  "enrolledDeviceCount": 1024,
  "qrCode": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```



