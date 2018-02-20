# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune_onboarding_devicemanagement_get.md)|[deviceManagement](../resources/intune_onboarding_devicemanagement.md)|Propriedades de leitura e relações do objeto [deviceManagement](../resources/intune_onboarding_devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune_onboarding_devicemanagement_update.md)|[deviceManagement](../resources/intune_onboarding_devicemanagement.md)|Atualiza as propriedades de um objeto [deviceManagement](../resources/intune_onboarding_devicemanagement.md).|
|[Função verifyWindowsEnrollmentAutoDiscovery](../api/intune_onboarding_devicemanagement_verifywindowsenrollmentautodiscovery.md)|Booliano|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|
|intuneBrand|[intuneBrand](../resources/intune_onboarding_intunebrand.md)|intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceCategories|Coleção [deviceCategory](../resources/intune_onboarding_devicecategory.md)|A lista de categorias de dispositivo com o locatário.|
|exchangeConnectors|Coleção [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)|A lista dos Conectores do Exchange configurados pelo locatário.|
|deviceEnrollmentConfigurations|Coleção [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|A lista de configurações de registro de dispositivos|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|As configurações de acesso condicional do Exchange no local. O acesso condicional no local exigirá que os dispositivos sejam registrados e estejam em conformidade para o acesso ao email|
|mobileThreatDefenseConnectors|Coleção [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|A lista dos conectores de defesa contra ameaças móveis configurados pelo locatário.|
|deviceManagementPartners|Coleção [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|A lista de Parceiros de gerenciamento de dispositivos configurados pelo locatário.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "intuneBrand": {
    "@odata.type": "microsoft.graph.intuneBrand",
    "displayName": "String",
    "contactITName": "String",
    "contactITPhoneNumber": "String",
    "contactITEmailAddress": "String",
    "contactITNotes": "String",
    "privacyUrl": "String",
    "onlineSupportSiteUrl": "String",
    "onlineSupportSiteName": "String",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1024,
      "g": 1024,
      "b": 1024
    },
    "showLogo": true,
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "String",
      "value": "binary"
    },
    "darkBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "String",
      "value": "binary"
    },
    "showNameNextToLogo": true,
    "showDisplayNameNextToLogo": true
  }
}
```



