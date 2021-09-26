---
title: tipo de recurso de dispositivo
description: Representa um dispositivo registrado no diretório.
ms.localizationpriority: medium
author: spunukol
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: db958d3789e0e98f19e258d6f833206ade738f5c
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763052"
---
# <a name="device-resource-type"></a>tipo de recurso de dispositivo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um dispositivo registrado no diretório. Dispositivos são criados na nuvem usando o Serviço de Registro de Dispositivo ou por meio do Intune. Eles são usados por políticas de acesso condicional para a autenticação multifator. Estes dispositivos podem variar desde computadores desktop e laptops até telefones e tablets. Herda de [directoryObject](directoryobject.md).

Esse recurso permite que você adicione seus próprios dados às propriedades personalizadas usando [extensions](/graph/extensibility-overview).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter dispositivo](../api/device-get.md) | [device](device.md) |Ler propriedades e relações do objeto device.|
|[Listar dispositivos](../api/device-list.md) | Coleção [device](device.md)| Recupere uma lista de dispositivos registrados no diretório. |
|[Atualizar dispositivo](../api/device-update.md) | [device](device.md)  |Atualize as propriedades do objeto device. |
|[Excluir dispositivo](../api/device-delete.md) | Nenhuma |Exclua o objeto device. |
|[Listar memberOf](../api/device-list-memberof.md) |Coleção [directoryObject](directoryobject.md)| Listar os grupos dos que o dispositivo é um membro direto. |
|[Listar memberOf transitivos](../api/device-list-transitivememberof.md) |Coleção [directoryObject](directoryobject.md)| Listar os grupos dos que o dispositivo é membro. Esta operação é transitiva. |
|[Listar registeredOwners](../api/device-list-registeredowners.md) |Coleção [directoryObject](directoryobject.md)| Obtenha os usuários que são proprietários registrados do dispositivo da propriedade de navegação registeredOwners.|
|[Listar registeredUsers](../api/device-list-registeredusers.md) |Coleção [directoryObject](directoryobject.md)| Obtenha os usuários registrados do dispositivo da propriedade de navegação registeredUsers.|
|[List usageRights](../api/device-list-usagerights.md) | Coleção [usageRight](usageright.md) | Obter uma coleção de direitos de uso concedidos ao dispositivo.|
|[checkMemberObjects](../api/device-checkmemberobjects.md) | Coleção de cadeias de caracteres | Verifique se há associação em uma lista de grupos, função de diretório ou objetos de unidade administrativa. |
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) || Criar uma definição para a extensão de esquema e usá-la para adicionar dados digitados personalizados a um recurso.|

## <a name="properties"></a>Propriedades

> [!IMPORTANT]
> O uso específico de `$filter` e o parâmetro de consulta `$search` é suportado somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`. Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|accountEnabled|Booliano| `true` se a conta estiver habilitada; caso contrário, `false`. O padrão é `true`. <br/><br/> Suporta `$filter` (`eq`, `ne`, `NOT`, `in`). Somente chamadores nas funções Administrador Global e Administrador de Dispositivos de Nuvem podem definir essa propriedade.|
|alternativeSecurityIds|Coleção [alternativeSecurityId](alternativeSecurityId.md)| Apenas para uso interno. Não anulável. Suporta `$filter` (`eq`, `NOT`, `ge`, `le`). |
|approximateLastSignInDateTime|DateTimeOffset| O tipo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. Suporta `$filter` ( , , , , ) e `eq` `ne` `NOT` `ge` `le` `$orderBy` . |
|complianceExpirationDateTime|DateTimeOffset| O timestamp quando o dispositivo não é mais considerado compatível. O tipo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |
|deviceCategory|String|Propriedade definida pelo usuário definida pelo Intune para adicionar automaticamente dispositivos a grupos e simplificar o gerenciamento de dispositivos.|
|deviceId|Cadeia de caracteres| Identificador definido pelo Serviço de Registro de Dispositivo do Azure no momento do registro. Suporta `$filter` (`eq`, `ne`, `NOT`, `startsWith`). |
|deviceMetadata|String| Apenas para uso interno. Definido como `null`. |
|deviceOwnership|Cadeia de caracteres|Propriedade do dispositivo. Essa propriedade é definida pelo Intune. Os valores possíveis são: `unknown`, `company`, `personal`.|
|deviceVersion|Int32| Apenas para uso interno. |
|displayName|Cadeia de caracteres| O nome de exibição do dispositivo. Obrigatório. Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`), `$search`, e `$orderBy`.  |
|domainName|Cadeia de caracteres|O nome de domínio local dos dispositivos ingressados no Azure AD híbrido. Essa propriedade é definida pelo Intune.|
|enrollmentProfileName|String|Perfil de registro aplicado ao dispositivo. Por exemplo, `Apple Device Enrollment Profile` , `Device enrollment - Corporate device identifiers` ou `Windows Autopilot profile name` . Essa propriedade é definida pelo Intune.|
|enrollmentType|String|Tipo de registro do dispositivo. Essa propriedade é definida pelo Intune. Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|id|Cadeia de caracteres|O identificador exclusivo do dispositivo. Herdado de [directoryObject](directoryobject.md). Chave, Não anulável. Somente leitura. Suporta `$filter` (`eq`, `ne`, `NOT`, `in`). |
|isCompliant|Booliano|`true` se o dispositivo estiver em conformidade com políticas de Gerenciamento de Dispositivo Móvel (MDM); caso contrário, `false` . Somente leitura. Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional de dispositivo ou por um [aplicativo MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para Windows do sistema operacional. Suporta `$filter` (`eq`, `ne`, `NOT`).|
|isManaged|Booliano|`true` se o dispositivo for gerenciado por um aplicativo MDM (Gerenciamento de Dispositivo Móvel). caso contrário, `false` . Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional de dispositivo ou por um [aplicativo MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para Windows do sistema operacional. Suporta `$filter` (`eq`, `ne`, `NOT`). |
|isRooted|Boolean|`true` se o dispositivo estiver enraizado; `false` se o dispositivo estiver com a cadeia quebrada. Isso só pode ser atualizado pelo Intune.|
|managementType|String|Canal de gerenciamento do dispositivo.  Essa propriedade é definida pelo Intune. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.|
|fabricante|String| Fabricante do dispositivo. Somente leitura. |
|mdmAppId|Cadeia de caracteres|Identificador de aplicativo usado para registrar o dispositivo no MDM. Somente leitura. Suporta `$filter` (`eq`, `ne`, `NOT`, `startsWith`).|
|modelo|String| Modelo do dispositivo. Somente leitura. |
|onPremisesLastSyncDateTime|DateTimeOffset|A última vez em que o objeto foi sincronizado com o diretório local. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z` somente leitura. Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`). |
|onPremisesSyncEnabled|Booliano|`true` se esse objeto está sincronizado de um diretório local; `false` se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; `null` se esse objeto nunca foi sido sincronizado de um diretório local (padrão).  Somente leitura. Suporta `$filter` (`eq`, `ne`, `NOT`, `in`). |
|operatingSystem|String| O tipo de sistema operacional do dispositivo. Obrigatório. Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `startsWith`). |
|operatingSystemVersion|String| A versão do sistema operacional do dispositivo. Obrigatório. Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `startsWith`). |
|physicalIds|Coleção de cadeias de caracteres| Apenas para uso interno. Não anulável. Suporta `$filter` (`eq`, `NOT`, `ge`, `le`, `startsWith`). |
|profileType|Cadeia de caracteres|O tipo de perfil do dispositivo. Valores possíveis: `RegisteredDevice` (padrão), `SecureVM` , , , `Printer` `Shared` `IoT` .|
|registrationDateTime|DateTimeOffset|Data e hora de quando o dispositivo foi registrado. O tipo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|systemLabels|Coleção de cadeias de caracteres| Lista de rótulos aplicados ao dispositivo pelo sistema. |
|hostnames|Coleção de cadeias de caracteres| Lista de hostNames do dispositivo.|
|trustType|Cadeia de caracteres| Tipo de relação de confiança para o dispositivo associado. Somente leitura. Valores possíveis: (indica trazer seus próprios dispositivos pessoais ), (Dispositivos ingressados apenas na nuvem) (dispositivos ingressados no domínio local `Workplace`  `AzureAd` `ServerAd` ingressados no Azure AD). Saiba mais em [Introdução ao gerenciamento de dispositivo no Azure Active Directory](/azure/active-directory/device-management-introduction) |
|name| Cadeia de caracteres | Nome amigável de um dispositivo. Somente retornado se o usuário entrar com uma conta da Microsoft como parte Project Roma. |
|status | String| O dispositivo é `online` ou `offline` . Somente retornado se o usuário entrar com uma conta da Microsoft como parte Project Roma. |
|plataforma |Cadeia de caracteres|Plataforma do dispositivo. Somente retornado se o usuário entrar com uma conta da Microsoft como parte Project Roma. Somente retornado se o usuário entrar com uma conta da Microsoft como parte Project Roma.|
|Tipo| String| Fator de formulário do dispositivo. Somente retornado se o usuário entrar com uma conta da Microsoft como parte Project Roma. |
|modelo| String| Modelo de dispositivo. Somente retornado se o usuário entrar com uma conta da Microsoft como parte Project Roma. |
|fabricante| String| Fabricante do dispositivo. Somente retornado se o usuário entrar com uma conta da Microsoft como parte Project Roma. |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| comandos | [coleção command](command.md) | Conjunto de comandos enviados para este dispositivo.|
|extensions|[extension](extension.md) collection|A coleção de extensões abertas definidas para o dispositivo. Somente leitura. Anulável. |
|memberOf|Coleção [directoryObject](directoryobject.md)|Grupos dos que esse dispositivo é membro. Somente leitura. Anulável. Suporta o `$expand`. |
|registeredOwners|Coleção [directoryObject](directoryobject.md)| O usuário que associou o dispositivo na nuvem ou registrou seu dispositivo pessoal. O proprietário registrado é definido no momento do registro. Atualmente, só pode haver um proprietário. Somente leitura. Anulável. Suporta o `$expand`. |
|registeredUsers|Coleção [directoryObject](directoryobject.md)| Coleção de usuários registrados do dispositivo. Para dispositivos associados em nuvem e dispositivos pessoais registrados, os usuários registrados são definidos para o mesmo valor que proprietários registrados no momento do registro. Somente leitura. Anulável. Suporta o `$expand`. |
|transitiveMemberOf |Coleção [directoryObject](directoryobject.md)| Grupos dos que esse dispositivo é membro. Esta operação é transitiva. Suporta o `$expand`.  |
|usageRights|Coleção [usageRight](usageright.md)|Representa os direitos de uso que um dispositivo recebeu. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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
  "approximateLastSignInDateTime": "String (timestamp)",
  "complianceExpirationDateTime": "String (timestamp)",
  "deviceCategory": "string",
  "deviceId": "string",
  "deviceMetadata": "string",
  "deviceOwnership": "string",
  "deviceVersion": 1024,
  "displayName": "string",
  "domainName": "string",
  "enrollmentProfileName": "string",
  "enrollmentType": "string",
  "id": "string (identifier)",
  "isCompliant": true,
  "isManaged": true,
  "isRooted": true,
  "mdmAppId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "string",
  "operatingSystemVersion": "string",
  "physicalIds": ["string"],
  "profileType": "string",
  "registrationDateTime": "String (timestamp)",
  "systemLabels": ["string"],
  "hostNames" : ["string"],
  "trustType": "string",
  "Name": "string",
  "Status": "string",
  "Platform": "string",
  "Kind": "string",
  "Model": "string",
  "managementType": "string",
  "Manufacturer": "string"
}
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
