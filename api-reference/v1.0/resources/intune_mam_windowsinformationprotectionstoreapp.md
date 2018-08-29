# <a name="windowsinformationprotectionstoreapp-resource-type"></a>Tipo de recurso windowsInformationProtectionStoreApp

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Aplicativo de loja para proteção de informações do Windows

Herdado de [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição do aplicativo. Herdado de [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|
|descrição|Cadeia de caracteres|A descrição do aplicativo. Herdado de [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|
|publisherName|Cadeia de caracteres|O nome do fornecedor herdado de [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|
|productName|Cadeia de caracteres|O nome do produto. Herdado de [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|
|negado|Booliano|Se verdadeiro, é negada proteção ou isenção ao aplicativo. Herdado de [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.windowsInformationProtectionApp",
  "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionStoreApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



