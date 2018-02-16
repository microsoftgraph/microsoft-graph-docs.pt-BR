# <a name="androidforworksettings-resource-type"></a>Tipo de recurso androidForWorkSettings

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configurações para o Android for Work.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter androidForWorkSettings](../api/intune_androidforwork_androidforworksettings_get.md)|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)|Ler propriedades e relações de objetos de [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md).|
|[Atualizar androidForWorkSettings](../api/intune_androidforwork_androidforworksettings_update.md)|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)|Atualizar as propriedades de um objeto de [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md).|
|[Ação requestSignupUrl](../api/intune_androidforwork_androidforworksettings_requestsignupurl.md)|Cadeia de caracteres|Gera uma URL de inscrição usada para se inscrever no gerenciamento do Android for Work.|
|[Ação completeSignup](../api/intune_androidforwork_androidforworksettings_completesignup.md)|Nenhum|Conclui o fluxo de inscrição para gerenciamento do Android for Work.|
|[Ação syncApps](../api/intune_androidforwork_androidforworksettings_syncapps.md)|Nenhum|Sincroniza aplicativos aprovados para a empresa.|
|[Ação de desvincular](../api/intune_androidforwork_androidforworksettings_unbind.md)|Nenhum|Desabilita o gerenciamento do Android for Work para a empresa.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de configurações do Android for Work|
|bindStatus|Cadeia de caracteres|Associa o status do locatário com a API do Google EMM Os valores possíveis são: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Hora da conclusão da última sincronização do aplicativo|
|lastAppSyncStatus|Cadeia de caracteres|Resultado da última sincronização do aplicativo Os valores possíveis são: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|Cadeia de caracteres|UPN proprietária que criou a empresa|
|ownerOrganizationName|Cadeia de caracteres|Nome da organização usada ao integrar o Android for Work|
|lastModifiedDateTime|DateTimeOffset|Hora da última modificação das configurações do Android for Work|
|enrollmentTarget|Cadeia de caracteres|Indica quais usuários podem registrar dispositivos no gerenciamento de dispositivos do Android for Work Os valores possíveis são: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|Conjunto de cadeia de caracteres|Especifica a quais grupos AAD podem registrar dispositivos no gerenciamento de dispositivos do Android for Work se enrollmentTarget estiver definido como 'Direcionado'|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ]
}
```



