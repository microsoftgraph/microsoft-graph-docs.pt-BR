# <a name="termsandconditionsacceptancestatus-resource-type"></a>Tipo de recurso termsAndConditionsAcceptanceStatus

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma entidade termsAndConditionsAcceptanceStatus representa o status de aceitação de uma política de Termos e Condições (T&C) por um determinado usuário. Os usuários devem aceitar a versão mais recente dos termos para manterem o acesso ao Portal da Empresa.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar termsAndConditionsAcceptanceStatuses](../api/intune_companyterms_termsandconditionsacceptancestatus_list.md)|Coleção [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|Lista propriedades e relações do objeto [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).|
|[Obter termsAndConditionsAcceptanceStatus](../api/intune_companyterms_termsandconditionsacceptancestatus_get.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|Propriedades de leitura e relações do objeto [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).|
|[Criar termsAndConditionsAcceptanceStatus](../api/intune_companyterms_termsandconditionsacceptancestatus_create.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|Cria um novo objeto [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).|
|[Excluir termsAndConditionsAcceptanceStatus](../api/intune_companyterms_termsandconditionsacceptancestatus_delete.md)|Nenhuma|Exclui um [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).|
|[Atualizar termsAndConditionsAcceptanceStatus](../api/intune_companyterms_termsandconditionsacceptancestatus_update.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|Atualiza as propriedades de um objeto [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da entidade.|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário cuja aceitação a entidade representa.|
|acceptedVersion|Int32|Número da versão mais recente dos T&C aceitos pelo usuário.|
|acceptedDateTime|DateTimeOffset|A data e a hora em que os termos foram aceitos pela última vez pelo usuário.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|Link de navegação para os termos e condições atribuídos.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```



