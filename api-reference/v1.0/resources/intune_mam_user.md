# <a name="user-resource-type"></a>Tipo de recurso de usuário

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa um objeto de usuário do Azure Active Directory.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar usuários](../api/intune_mam_user_list.md)|Conjunto [user](../resources/intune_mam_user.md)|Listar propriedades e relações de objetos de [user](../resources/intune_mam_user.md).|
|[Obter usuário](../api/intune_mam_user_get.md)|[user](../resources/intune_mam_user.md)|Ler propriedades e relações de objetos de [user](../resources/intune_mam_user.md).|
|[Criar usuário](../api/intune_mam_user_create.md)|[user](../resources/intune_mam_user.md)|Criar um novo objeto de [user](../resources/intune_mam_user.md).|
|[Excluir usuário](../api/intune_mam_user_delete.md)|Nenhum|Excluir [user](../resources/intune_mam_user.md).|
|[Atualizar user](../api/intune_mam_user_update.md)|[user](../resources/intune_mam_user.md)|Atualizar as propriedades de um objeto de [user](../resources/intune_mam_user.md).|
|[função getManagedAppDiagnosticStatuses](../api/intune_mam_user_getmanagedappdiagnosticstatuses.md)|Conjunto [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md)|Obtém diagnóstico do status de validação para um determinado usuário.|
|[Função getManagedAppPolicies](../api/intune_mam_user_getmanagedapppolicies.md)|Conjunto [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Obtém as restrições de aplicativo para um determinado usuário.|
|[Ação wipeManagedAppRegistrationsByDeviceTag](../api/intune_mam_user_wipemanagedappregistrationsbydevicetag.md)|Nenhum|Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador do usuário.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedAppRegistrations|Conjunto [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|Zero ou mais registros de aplicativos gerenciados que pertencem ao usuário.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



