# <a name="userinstallstatesummary-resource-type"></a>Tipo de recurso userInstallStateSummary

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém as propriedades do resumo de estado de instalação de um usuário.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userInstallStateSummaries](../api/intune_books_userinstallstatesummary_list.md)|Conjunto [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|Listar propriedades e relações de objetos de [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).|
|[Obter userInstallStateSummary](../api/intune_books_userinstallstatesummary_get.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|Ler propriedades e relações de objetos de [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).|
|[Criar userInstallStateSummary](../api/intune_books_userinstallstatesummary_create.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|Criar um novo objeto de [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).|
|[Excluir userInstallStateSummary](../api/intune_books_userinstallstatesummary_delete.md)|Nenhum|Excluir [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).|
|[Atualizar userInstallStateSummary](../api/intune_books_userinstallstatesummary_update.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|Atualizar as propriedades de um objeto de [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|userName|Cadeia de caracteres|Nome do usuário.|
|installedDeviceCount|Int32|Contagem de dispositivos instalados.|
|failedDeviceCount|Int32|Falha na contagem de dispositivos.|
|notInstalledDeviceCount|Int32|Sem contagem de dispositivos instalados.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceStates|Conjunto [deviceInstallState](../resources/intune_books_deviceinstallstate.md)|O estado de instalação do livro eletrônico.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userInstallStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "String (identifier)",
  "userName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```



