---
title: tipo de recurso de dispositivo
description: Representa um dispositivo registrado no diretório.
localization_priority: Normal
author: spunukol
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 34fc75c74d0c48edda5ca69cb4cc27bbfc78b48c
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943581"
---
# <a name="device-resource-type"></a>tipo de recurso de dispositivo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um dispositivo registrado no diretório. Dispositivos são criados na nuvem usando o Serviço de Registro de Dispositivo ou por meio do Intune. Eles são usados por políticas de acesso condicional para a autenticação multifator. Estes dispositivos podem variar desde computadores desktop e laptops até telefones e tablets. Herda de [directoryObject](directoryobject.md).

Esse recurso permite que você adicione seus próprios dados às propriedades personalizadas usando [extensions](/graph/extensibility-overview).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter dispositivo](../api/device-get.md) | [device](device.md) |Leia as propriedades e os relacionamentos do objeto device.|
|[Listar dispositivos](../api/device-list.md) | Coleção [device](device.md)| Recupere uma lista de dispositivos registrados no diretório. |
|[Atualizar dispositivo](../api/device-update.md) | [device](device.md)  |Atualize as propriedades do objeto device. |
|[Excluir dispositivo](../api/device-delete.md) | Nenhuma |Exclua o objeto device. |
|[Listar memberOf](../api/device-list-memberof.md) |Coleção [directoryObject](directoryobject.md)| Liste os grupos dos que o dispositivo é membro direto. |
|[Listar memberOf transitivos](../api/device-list-transitivememberof.md) |Coleção [directoryObject](directoryobject.md)| Listar os grupos dos que o dispositivo é membro. Esta operação é transitiva. |
|[Listar registeredOwners](../api/device-list-registeredowners.md) |Coleção [directoryObject](directoryobject.md)| Obtenha os usuários que são proprietários registrados do dispositivo da propriedade de navegação registeredOwners.|
|[Listar registeredUsers](../api/device-list-registeredusers.md) |Coleção [directoryObject](directoryobject.md)| Obtenha os usuários registrados do dispositivo da propriedade de navegação registeredUsers.|
|[Listar usageRights](../api/device-list-usagerights.md) | [coleção usageRight](usageright.md) | Obter uma coleção de direitos de uso concedidos ao dispositivo.|
|[checkMemberObjects](../api/device-checkmemberobjects.md) | Coleção de cadeias de caracteres | Verifique se há associação em uma lista de grupos, função de diretório ou objetos de unidade administrativa. |
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) || Criar uma definição para a extensão de esquema e usá-la para adicionar dados digitados personalizados a um recurso.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|accountEnabled|Booliano| **true** se a conta estiver habilitada; caso contrário, **false**. padrão é true.|
|alternativeSecurityIds|Coleção alternativeSecurityId| Apenas para uso interno. Não anulável. |
|approximateLastSignInDateTime|DateTimeOffset| O tipo timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura. |
|complianceExpirationDateTime|DateTimeOffset| O timestamp quando o dispositivo não é mais considerado compatível. O tipo timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura. |
|deviceId|Guid| Identificador exclusivo definido pelo serviço de registro do dispositivo Azure no momento do registro. |
|deviceMetadata|String| Apenas para uso interno. Definido como nulo. |
|deviceVersion|Int32| Apenas para uso interno. |
|displayName|String| O nome de exibição do dispositivo. Obrigatório. |
|id|String|O identificador exclusivo do dispositivo. Herdado de [directoryObject](directoryobject.md). Chave, Não anulável. Somente leitura.|
|isCompliant|Booliano|**True** se o dispositivo está em conformidade com políticas de MDM (Gerenciamento de Dispositivo Móvel); caso contrário, **false**. Somente leitura. Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional de dispositivo ou por um [aplicativo MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para dispositivos do sistema operacional Windows.|
|isManaged|Booliano|**true** se o dispositivo for gerenciado por um aplicativo de gerenciamento de dispositivo móvel (MDM); caso contrário, **false**. Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional de dispositivo ou por um [aplicativo MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para dispositivos do sistema operacional Windows. |
|fabricante|String| Fabricante do dispositivo. Somente leitura. |
|mdmAppId|String|Identificador de aplicativo usado para registrar o dispositivo no MDM. <br><br>Somente leitura. Oferece suporte a $filter.|
|modelo|String| Modelo do dispositivo. Somente leitura. |
|onPremisesLastSyncDateTime|DateTimeOffset|A última vez em que o objeto foi sincronizado com o diretório local. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'` Somente leitura. |
|onPremisesSyncEnabled|Booliano|**True** se esse objeto está sincronizado de um diretório local; **false** se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão). Somente leitura.|
|operatingSystem|String| O tipo de sistema operacional do dispositivo. Obrigatório. |
|operatingSystemVersion|String| A versão do sistema operacional do dispositivo. Obrigatório. |
|physicalIds|Coleção de cadeias de caracteres| Apenas para uso interno. Não anulável. |
|profileType|String|O tipo de perfil do dispositivo. Valores possíveis:<br />**RegisteredDevice** (padrão)<br />**SecureVM**<br />**Printer**<br />**Compartilhado**<br />**IoT**|
|systemLabels|Coleção de cadeias de caracteres| Lista de rótulos aplicados ao dispositivo pelo sistema. |
|hostNames|Coleção de cadeias de caracteres| Lista de hostNames para o dispositivo.|
|trustType|Cadeia de caracteres| Tipo de relação de confiança para o dispositivo associado. Somente leitura. Valores possíveis: <br />**Workplace** – indica *traga seus dispositivos pessoais*<br />**AzureAd** – apenas dispositivos associados na nuvem<br />**ServerAd** – dispositivos associados no domínio local unidos ao Azure AD. Saiba mais em [Introdução ao gerenciamento de dispositivo no Azure Active Directory](/azure/active-directory/device-management-introduction) |
|Nome| String | Nome amigável de um dispositivo. Retornado somente se o usuário entrar com uma conta da Microsoft como parte do Projeto Roma. |
|Status | String| O dispositivo está online ou offline. Retornado somente se o usuário entrar com uma conta da Microsoft como parte do Projeto Roma. |
|Plataforma |String|Plataforma do dispositivo. Retornado somente se o usuário entrar com uma conta da Microsoft como parte do Projeto Roma. Retornado somente se o usuário entrar com uma conta da Microsoft como parte do Projeto Roma.|
|Tipo| String| Fator forma do dispositivo. Retornado somente se o usuário entrar com uma conta da Microsoft como parte do Projeto Roma. |
|Modelo| String| Modelo do dispositivo. Retornado somente se o usuário entrar com uma conta da Microsoft como parte do Projeto Roma. |
|Fabricante| String| Fabricante do dispositivo. Retornado somente se o usuário entrar com uma conta da Microsoft como parte do Projeto Roma. |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para o dispositivo. Somente leitura. Anulável.|
|registeredOwners|Coleção [directoryObject](directoryobject.md)| O usuário que associou o dispositivo na nuvem ou registrou seu dispositivo pessoal. O proprietário registrado é definido no momento do registro. Atualmente, só pode haver um proprietário. Somente leitura. Anulável.|
|registeredUsers|Coleção [directoryObject](directoryobject.md)| Coleção de usuários registrados do dispositivo. Para dispositivos associados em nuvem e dispositivos pessoais registrados, os usuários registrados são definidos para o mesmo valor que proprietários registrados no momento do registro. Somente leitura. Anulável.|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para o dispositivo. Anulável.|
|registeredOwners|Coleção [directoryObject](directoryobject.md)|Usuários que são proprietários registrados do dispositivo. Somente leitura. Anulável.|
|registeredUsers|Coleção [directoryObject](directoryobject.md)|Usuários que são usuários registrados do dispositivo. Somente leitura. Anulável.|
| comandos | [coleção de](command.md) comandos | Conjunto de comandos enviados para este dispositivo|
|usageRight|[coleção usageRight](usageright.md)|Representa os direitos de uso que um dispositivo recebeu. |

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
  "deviceId": "string",
  "deviceMetadata": "string",
  "deviceVersion": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "isCompliant": true,
  "isManaged": true,
  "mdmAppId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "string",
  "operatingSystemVersion": "string",
  "physicalIds": ["string"],
  "profileType": "string",
  "systemLabels": ["string"],
  "hostNames" : ["string"],
  "trustType": "string",
  "Name": "string",
  "Status": "string",
  "Platform": "string",
  "Kind": "string",
  "Model": "string",
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
