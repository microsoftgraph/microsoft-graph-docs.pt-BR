# <a name="managedapppolicydeploymentsummary-resource-type"></a>Tipo de recurso managedAppPolicyDeploymentSummary

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter managedAppPolicyDeploymentSummary](../api/intune_mam_managedapppolicydeploymentsummary_get.md)|[managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md)|Ler propriedades e relações de objetos de [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md).|
|[Atualizar managedAppPolicyDeploymentSummary](../api/intune_mam_managedapppolicydeploymentsummary_update.md)|[managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md)|Atualizar as propriedades de um objeto de [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Ainda não documentado|
|configurationDeployedUserCount|Int32|Ainda não documentado|
|lastRefreshTime|DateTimeOffset|Ainda não documentado|
|configurationDeploymentSummaryPerApp|Conjunto [managedAppPolicyDeploymentSummaryPerApp](../resources/intune_mam_managedapppolicydeploymentsummaryperapp.md)|Ainda não documentado|
|id|Cadeia de caracteres|Chave da entidade.|
|version|Cadeia de caracteres|Versão da entidade.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "String",
  "configurationDeployedUserCount": 1024,
  "lastRefreshTime": "String (timestamp)",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "String"
      },
      "configurationAppliedUserCount": 1024
    }
  ],
  "id": "String (identifier)",
  "version": "String"
}
```



