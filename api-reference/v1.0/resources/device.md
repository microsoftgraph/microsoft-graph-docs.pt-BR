# <a name="device-resource-type"></a>tipo de recurso de dispositivo

Representa um dispositivo registrado na organização. Dispositivos também podem ser criados na nuvem usando o Serviço de Registro de Dispositivo ou por meio do Intune. Eles são utilizados por políticas de acesso condicional para autenticação de vários fatores. Estes dispositivos podem variar desde computadores desktop e laptops até telefones e tablets. Herda de [directoryObject](directoryobject.md).

Esse recurso permite que você adicione seus próprios dados às propriedades personalizadas usando [extensions](../../../concepts/extensibility_overview.md).


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Create device](../api/device_post_devices.md) | [device](device.md) |Crie um novo dispositivo registrado no diretório.|
|[Obter dispositivo](../api/device_get.md) | [device](device.md) |Leia as propriedades e os relacionamentos de um objeto device.|
|[Listar dispositivos](../api/device_list.md) | Coleção [device](device.md)| Recupere uma lista de dispositivos registrados no diretório. |
|[Atualizar dispositivo](../api/device_update.md) | [device](device.md) |Atualize as propriedades de um objeto device. |
|[Excluir dispositivo](../api/device_delete.md) | Nenhuma |Exclua um objeto device. |
|[Criar registeredOwner](../api/device_post_registeredowners.md) |[directoryObject](directoryobject.md)| Adicione um usuário como um novo proprietário do dispositivo postando na propriedade de navegação registeredOwners.|
|[Listar registeredOwners](../api/device_list_registeredowners.md) |Coleção [directoryObject](directoryobject.md)| Obtenha os usuários que são proprietários registrados do dispositivo da propriedade de navegação registeredOwners.|
|[Criar registeredUser](../api/device_post_registeredusers.md) |[directoryObject](directoryobject.md)| Adicione um usuário registrado para o dispositivo postando na propriedade de navegação registeredUsers.|
|[Listar registeredUsers](../api/device_list_registeredusers.md) |Coleção [directoryObject](directoryobject.md)| Obtenha os usuários registrados do dispositivo da propriedade de navegação registeredUsers.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension_get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](../../../concepts/extensibility_schema_groups.md) || Crie uma definição para a extensão de esquema e use-a para adicionar dados digitados personalizados a um recurso.|

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|accountEnabled|Booliano| **true** se a conta estiver habilitada; caso contrário, **false**. Obrigatório.|
|alternativeSecurityIds|Coleção [alternativeSecurityId](alternativesecurityid.md)| O operador **any** é necessário para expressões de filtro em propriedades de vários valores. Não anulável. Obrigatório. |
|approximateLastSignInDateTime|DateTimeOffset| O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|deviceId|Guid| GUID exclusivo especificado pelo cliente para representar o dispositivo. Obrigatório. |
|deviceMetadata|String|    |
|deviceVersion|Int32|            |
|displayName|String|O nome de exibição do dispositivo. Obrigatório. |
|id|String|O identificador exclusivo do dispositivo. Herdado de [directoryObject](directoryobject.md). Chave, Não anulável. Somente leitura.|
|isCompliant|Booliano|**True** se o dispositivo está em conformidade com políticas de MDM (Gerenciamento de Dispositivo Móvel); caso contrário, **false**.|
|isManaged|Booliano|**True** se o dispositivo é gerenciado por um aplicativo de gerenciamento de dispositivo móvel (MDM), como o Intune; caso contrário, **false**.|
|onPremisesLastSyncDateTime|DateTimeOffset|A última vez em que o objeto foi sincronizado com o diretório local. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|onPremisesSyncEnabled|Boolean|**True** se esse objeto está sincronizado de um diretório local; **false** se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão).|
|operatingSystem|String|O tipo de sistema operacional do dispositivo. Obrigatório. |
|operatingSystemVersion|String|A versão do sistema operacional do dispositivo. Obrigatório. |
|physicalIds|Coleção de cadeias de caracteres| Não anulável.            |
|trustType|String|    ||

## <a name="relationships"></a>Relações
| Relação | Tipo    |Descrição|
|:---------------|:--------|:----------|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para o dispositivo. Somente leitura. Anulável.|
|registeredOwners|Coleção [directoryObject](directoryobject.md)|Usuários que são proprietários registrados do dispositivo. Somente leitura. Anulável.|
|registeredUsers|Coleção [directoryObject](directoryobject.md)|Usuários que são usuários registrados do dispositivo. Somente leitura. Anulável.|



## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.device"
}-->

```json
{
  "accountEnabled": true,
  "alternativeSecurityIds": [{"@odata.type": "microsoft.graph.alternativeSecurityId"}],
  "approximateLastSignInDateTime": "String (timestamp)",
  "deviceId": "string",
  "deviceMetadata": "string",
  "deviceVersion": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "string",
  "operatingSystemVersion": "string",
  "physicalIds": ["string"],
  "trustType": "string"
}

```

## <a name="see-also"></a>Ver também

- [Adicionar dados personalizados a recursos usando extensões](../../../concepts/extensibility_overview.md)
- [Adicionar dados personalizados aos usuários usando extensões abertas](../../../concepts/extensibility_open_users.md)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
