---
title: tipo de recurso de dispositivo
description: Representa um dispositivo registrado no diretório.
ms.localizationpriority: medium
author: sandeo-MSFT
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 79aa81d4125cf51d52bb11a39d7fdd70514e8a91
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555664"
---
# <a name="device-resource-type"></a>tipo de recurso de dispositivo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um dispositivo registrado no diretório. Dispositivos são criados na nuvem usando o Serviço de Registro de Dispositivo ou por meio do Intune. Eles são usados por políticas de acesso condicional para a autenticação multifator. Estes dispositivos podem variar desde computadores desktop e laptops até telefones e tablets. Herda de [directoryObject](directoryobject.md).

Esse recurso é um tipo aberto que permite que outras propriedades sejam passadas. Você também pode adicionar seus próprios dados a propriedades [personalizadas como extensões](/graph/extensibility-overview).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter dispositivo](../api/device-get.md) | [device](device.md) |Ler propriedades e relações do objeto de dispositivo.|
|[Listar dispositivos](../api/device-list.md) | Coleção [device](device.md)| Recupere uma lista de dispositivos registrados no diretório. |
|[Atualizar dispositivo](../api/device-update.md) | [device](device.md)  |Atualize as propriedades do objeto do dispositivo. |
|[Excluir dispositivo](../api/device-delete.md) | Nenhuma |Exclua o objeto do dispositivo. |
|[Listar memberOf](../api/device-list-memberof.md) |Coleção [directoryObject](directoryobject.md)| Liste os grupos e unidades administrativas dos qual o dispositivo é membro direto. |
|[Listar memberOf transitivos](../api/device-list-transitivememberof.md) |Coleção [directoryObject](directoryobject.md)| Liste os grupos e unidades administrativas dos qual o dispositivo é membro. Esta operação é transitiva. |
|[Listar registeredOwners](../api/device-list-registeredowners.md) |Coleção [directoryObject](directoryobject.md)| Obtenha os usuários que são proprietários registrados do dispositivo da propriedade de navegação registeredOwners.|
|[Listar registeredUsers](../api/device-list-registeredusers.md) |Coleção [directoryObject](directoryobject.md)| Obtenha os usuários registrados do dispositivo da propriedade de navegação registeredUsers.|
|[List usageRights](../api/device-list-usagerights.md) | Coleção [usageRight](usageright.md) | Obtenha uma coleção de direitos de uso concedidos ao dispositivo.|
| [checkMemberGroups](../api/directoryobject-checkmembergroups.md) | Coleção de cadeias de caracteres | Verifique se há uma associação em uma lista de grupos. A verificação é transitiva. |
| [getMemberGroups](../api/directoryobject-getmembergroups.md) | Coleção de cadeias de caracteres | Retornar todos os grupos dos qual o dispositivo é membro. A verificação é transitiva. |
|[checkMemberObjects](../api/directoryobject-checkmemberobjects.md) | Coleção de cadeias de caracteres | Verifique se há associação em uma lista de grupos, função de diretório ou objetos de unidade administrativa. |
|[getMemberObjects](../api/directoryobject-checkmemberobjects.md) | Coleção de cadeias de caracteres | Retornar todos os grupos, unidades administrativas e funções de diretório dos qual o dispositivo é membro. A verificação é transitiva. |
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) || Criar uma definição para a extensão de esquema e usá-la para adicionar dados digitados personalizados a um recurso.|

## <a name="properties"></a>Propriedades

> [!IMPORTANT]
> O uso específico de `$filter` e o parâmetro de consulta `$search` é suportado somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`. Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries#device-properties).

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|accountEnabled|Booliano| `true` se a conta estiver habilitada; caso contrário, `false`. O padrão é `true`. <br/><br/> Suporta `$filter` (`eq`, `ne`, `not`, `in`). Somente chamadores nas funções administrador global e administrador de dispositivo de nuvem podem definir essa propriedade.|
|alternativeSecurityIds|Coleção [alternativeSecurityId](alternativeSecurityId.md)| Apenas para uso interno. Não anulável. Suporta `$filter` (`eq`, `not`, `ge`, `le`). |
|approximateLastSignInDateTime|DateTimeOffset| O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. Dá `$filter` suporte a (`eq`, `not``ne`, `ge`, `le`, e `eq` em `null` valores) e `$orderBy`. |
|complianceExpirationDateTime|DateTimeOffset| O carimbo de data/hora quando o dispositivo não é mais considerado compatível. O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |
|deviceCategory|String|Propriedade definida pelo usuário definida por Intune para adicionar automaticamente dispositivos a grupos e simplificar o gerenciamento de dispositivos.|
|deviceId|Cadeia de caracteres| Identificador definido pelo Serviço de Registro de Dispositivo do Azure no momento do registro. Suporta `$filter` (`eq`, `ne`, `not`, `startsWith`). |
|deviceMetadata|String| Apenas para uso interno. Definido como `null` |
|deviceOwnership|Cadeia de caracteres|Propriedade do dispositivo. Essa propriedade é definida por Intune. Os valores possíveis são: `unknown`, `company`, `personal`.|
|deviceVersion|Int32| Apenas para uso interno. |
|displayName|Cadeia de caracteres| O nome de exibição do dispositivo. Obrigatório. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores), `$search`, e `$orderBy`.  |
|domainName|Cadeia de caracteres|O nome de domínio local dos dispositivos ingressados Azure AD híbridos. Essa propriedade é definida por Intune.|
|enrollmentProfileName|String|Perfil de registro aplicado ao dispositivo. Por exemplo, `Apple Device Enrollment Profile`, `Device enrollment - Corporate device identifiers`ou `Windows Autopilot profile name`. Essa propriedade é definida por Intune.|
|enrollmentType|String|Tipo de registro do dispositivo. Essa propriedade é definida por Intune. Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
| extensionAttributes | [onPremisesExtensionAttributes](onpremisesextensionattributes.md) | Contém atributos de extensão de 1 a 15 para o dispositivo. Os atributos de extensão individuais não são selecionáveis. Essas propriedades são dominadas na nuvem e podem ser definidas durante a criação ou atualização de um objeto de dispositivo Azure AD. <br><br>Suporte `$filter` (`eq`, `not`, `startsWith`, e `eq` no `null` valores).|
|id|Cadeia de caracteres|O identificador exclusivo do dispositivo. Herdado de [directoryObject](directoryobject.md). Chave, Não anulável. Somente leitura. Suporta `$filter` (`eq`, `ne`, `not`, `in`). |
|isCompliant|Booliano|`true`se o dispositivo estiver em conformidade com as políticas de MDM (mobile Gerenciamento de Dispositivos), caso contrário, `false`. Somente leitura. Isso só pode ser atualizado por Intune para qualquer tipo de sistema operacional do dispositivo ou por um aplicativo [MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para dispositivos do sistema operacional Windows. Suporta `$filter` (`eq`, `ne`, `not`).|
|isManaged|Booliano|`true`se o dispositivo for gerenciado por um aplicativo MDM (mobile Gerenciamento de Dispositivos), caso contrário, `false`. Isso só pode ser atualizado por Intune para qualquer tipo de sistema operacional do dispositivo ou por um aplicativo [MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para dispositivos do sistema operacional Windows. Suporta `$filter` (`eq`, `ne`, `not`). |
|isRooted|Booliano|`true` se o dispositivo estiver com raiz; `false` se o dispositivo estiver com a cadeia quebrada. Isso só pode ser atualizado por Intune.|
|managementType|String|Canal de gerenciamento do dispositivo.  Essa propriedade é definida por Intune. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.|
|fabricante|String| Fabricante do dispositivo. Somente leitura. |
|mdmAppId|Cadeia de caracteres|Identificador de aplicativo usado para registrar o dispositivo no MDM. Somente leitura. Suporta `$filter` (`eq`, `ne`, `not`, `startsWith`).|
|modelo|String| Modelo do dispositivo. Somente leitura. |
|onPremisesLastSyncDateTime|DateTimeOffset|A última vez em que o objeto foi sincronizado com o diretório local. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z` somente leitura. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`). |
|onPremisesSyncEnabled|Booliano|`true` se esse objeto está sincronizado de um diretório local; `false` se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; `null` se esse objeto nunca foi sido sincronizado de um diretório local (padrão).  Somente leitura. Suporte `$filter` (`eq`, `ne`, `not`, `in`, e `eq` no `null` valores). |
|operatingSystem|String| O tipo de sistema operacional do dispositivo. Obrigatório. Dá `$filter` suporte (`eq`, `ne`, `not`, `ge`, `le`, `startsWith`e em `null` `eq` valores). |
|operatingSystemVersion|String| A versão do sistema operacional do dispositivo. Obrigatório. Dá `$filter` suporte (`eq`, `ne`, `not`, `ge`, `le`, `startsWith`e em `null` `eq` valores). |
|physicalIds|Coleção de cadeias de caracteres| Apenas para uso interno. Não anulável. Dá `$filter` suporte (`eq`, `not`, `ge`, `le`, `startsWith`e contando coleções vazias). |
|profileType|Cadeia de caracteres|O tipo de perfil do dispositivo. Valores possíveis: `RegisteredDevice` (padrão), `SecureVM`, `Printer`, `Shared`. `IoT`|
|registrationDateTime|DateTimeOffset|Data e hora de quando o dispositivo foi registrado. O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|systemLabels|Coleção de cadeias de caracteres| Lista de rótulos aplicados ao dispositivo pelo sistema. Dá `$filter` suporte (`eq` ao contar coleções vazias). |
|Hostnames|Coleção de cadeias de caracteres| Lista de hostNames para o dispositivo.|
|trustType|Cadeia de caracteres| Tipo de relação de confiança para o dispositivo associado. Somente leitura. Valores *possíveis:*`Workplace` (indica trazer seus próprios dispositivos pessoais), `AzureAd` (somente dispositivos ingressados na nuvem) `ServerAd` (dispositivos ingressados no domínio local ingressados no Azure AD). Saiba mais em [Introdução ao gerenciamento de dispositivo no Azure Active Directory](/azure/active-directory/device-management-introduction) |
|nome| Cadeia de caracteres | Nome amigável de um dispositivo. Retornado somente se o usuário entrar com uma conta da Microsoft como parte do Project Rome. |
|status | Cadeia de caracteres| O dispositivo é `online` ou `offline`. Retornado somente se o usuário entrar com uma conta da Microsoft como parte do Project Rome. |
|plataforma |Cadeia de caracteres|Plataforma do dispositivo. Retornado somente se o usuário entrar com uma conta da Microsoft como parte do Project Rome. Retornado somente se o usuário entrar com uma conta da Microsoft como parte do Project Rome.|
|Tipo| Cadeia de caracteres| Fator forma do dispositivo. Retornado somente se o usuário entrar com uma conta da Microsoft como parte do Project Rome. |
|modelo| String| Modelo de dispositivo. Retornado somente se o usuário entrar com uma conta da Microsoft como parte do Project Rome. |
|fabricante| String| Fabricante do dispositivo. Retornado somente se o usuário entrar com uma conta da Microsoft como parte do Project Rome. |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| comandos | [coleção de](command.md) comandos | Conjunto de comandos enviados para este dispositivo.|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para o dispositivo. Somente leitura. Anulável. |
|memberOf|Coleção [directoryObject](directoryobject.md)|Grupos e unidades administrativas das qual este dispositivo é membro. Somente leitura. Anulável. Suporta o `$expand`. |
|registeredOwners|Coleção [directoryObject](directoryobject.md)| O usuário que associou o dispositivo na nuvem ou registrou seu dispositivo pessoal. O proprietário registrado é definido no momento do registro. Atualmente, só pode haver um proprietário. Somente leitura. Anulável. Suporta o `$expand`. |
|registeredUsers|Coleção [directoryObject](directoryobject.md)| Coleção de usuários registrados do dispositivo. Para dispositivos associados em nuvem e dispositivos pessoais registrados, os usuários registrados são definidos para o mesmo valor que proprietários registrados no momento do registro. Somente leitura. Anulável. Suporta o `$expand`. |
|transitiveMemberOf |Coleção [directoryObject](directoryobject.md)| Grupos e unidades administrativas das qual este dispositivo é membro. Esta operação é transitiva. Suporta o `$expand`.  |
|Direitosdeuso|Coleção [usageRight](usageright.md)|Representa os direitos de uso que um dispositivo recebeu. |

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
  "extensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
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
