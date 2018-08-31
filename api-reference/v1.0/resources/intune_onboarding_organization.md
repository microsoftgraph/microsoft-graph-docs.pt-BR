# <a name="organization-resource-type"></a>tipo de recurso da organização

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar organizações](../api/intune_onboarding_organization_list.md)|Coleção [organization](../resources/intune_onboarding_organization.md)|Listar propriedades e relações de objetos de [organização](../resources/intune_onboarding_organization.md).|
|[Obter organização](../api/intune_onboarding_organization_get.md)|[organização](../resources/intune_onboarding_organization.md)|Ler propriedades e relações de objetos de [organização](../resources/intune_onboarding_organization.md).|
|[Atualizar a organização](../api/intune_onboarding_organization_update.md)|[organização](../resources/intune_onboarding_organization.md)|Atualizar as propriedades de um objeto de [organização](../resources/intune_onboarding_organization.md).|
|[Ação setMobileDeviceManagementAuthority](../api/intune_onboarding_organization_setmobiledevicemanagementauthority.md)|Int32|Define a autoridade de gerenciamento de dispositivo móvel|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto.|
|mobileDeviceManagementAuthority|[mdmAuthority](../resources/intune_onboarding_mdmauthority.md)|Autoridade de gerenciamento de dispositivo móvel. Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "openType": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.organization"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Resource microsoft.graph.organization is defined in multiple files: /api-reference/v1.0/resources/intune_onboarding_organization.md, /api-reference/v1.0/resources/organization.md"
  ]
}-->
