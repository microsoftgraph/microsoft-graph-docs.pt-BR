---
title: Tipo de recurso orgContact
description: Veja a seguir uma representação JSON do recurso
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 575a3d081c7b75b648890de6f0c9d91c2d1fdb24
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442905"
---
# <a name="orgcontact-resource-type"></a>Tipo de recurso orgContact

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um contato organizacional. Os contatos organizacionais são gerenciados pelos administradores de uma organização e são diferentes dos [contatos pessoais.](contact.md) Além disso, os contatos organizacionais são sincronizados de diretórios locais ou do Exchange Online e são somente leitura.

Herda de [directoryObject](directoryobject.md).

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/orgcontact-delta.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
| ------ | ----------- | ----------- |
| [Listar contatos organizacionais](../api/orgcontact-list.md) | [coleção orgContact](orgcontact.md) | Listar propriedades de contatos organizacionais. |
| [Obter contato organizacional](../api/orgcontact-get.md) | [orgContact](orgcontact.md) | Ler propriedades e relações do objeto orgContact. |
| [Obter gerenciador](../api/orgcontact-get-manager.md) | [directoryObject](directoryobject.md) | Obter o gerente do contato. |
| [Listar directReports](../api/orgcontact-list-directreports.md) | Coleção [directoryObject](directoryobject.md) | Listar os relatórios diretos do contato. |
| [Listar memberOf](../api/orgcontact-list-memberof.md) | Coleção [directoryObject](directoryobject.md) | Obter uma coleção de objetos memberOf. |
| [checkMemberGroups](../api/orgcontact-checkmembergroups.md) | Coleção de cadeias de caracteres | Verifique se há associação ao grupo. |
| [getMemberGroups](../api/orgcontact-getmembergroups.md) | Coleção de cadeias de caracteres | Retorne todos os grupos dos que o contato especificado é membro. |
| [getMemberObjects](../api/orgcontact-getmemberobjects.md) | Coleção de cadeias de caracteres | Retorna uma lista de directoryObjects do qual o contato é membro. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
| -------- | ---- | ----------- |
| addresses | [Coleção physicalOfficeAddress](physicalofficeaddress.md) | Endereços postais para esse contato organizacional. Por enquanto, um contato só pode ter um endereço físico. |
| companyName | String | Nome da empresa à que esse contato organizacional pertence. |
| department | String | O nome do departamento no qual o contato funciona. |
| displayName | String | Nome de exibição para esse contato organizacional. |
| givenName | String | Primeiro nome para esse contato organizacional. |
| id | String | Identificador exclusivo para esse contato organizacional. |
| jobTitle | String | Cargo para esse contato organizacional. |
| email | String | O endereço SMTP do contato, por exemplo, "jeff@contoso.onmicrosoft.com". |
| mailNickname | String | Alias de email (parte do endereço de email pré-pendente do símbolo @) para esse contato organizacional. |
| onPremisesLastSyncDateTime | DateTimeOffset | Data e hora em que esse contato organizacional foi sincronizado pela última vez do AD local. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| onPremisesProvisioningErrors | coleção [OnPremisesProvisioningError](onpremisesprovisioningerror.md) | Lista de erros de provisionamento de sincronização para esse contato organizacional. |
| onPremisesSyncEnabled | Booliano | **true** se esse objeto for sincronizado de um diretório local; **false** se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado e agora mestre no Exchange; **null** se esse objeto nunca tiver sido sincronizado de um diretório local (padrão). |
| telefones | Coleção [phone](phone.md) | Lista de telefones para esse contato organizacional. Os tipos de telefone podem ser móveis, comerciais e businessFax. Somente um de cada tipo pode estar presente na coleção. |
| proxyAddresses | Coleção de cadeias de caracteres | Por exemplo: "SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com". O operador **any** é obrigatório para expressões de filtro em propriedades de vários valores. Oferece suporte a $filter. |
| surname | String | Sobrenome para esse contato organizacional. |

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
| ------------ | ---- | ----------- |
| directReports | Coleção [directoryObject](directoryobject.md) | Os relatórios diretos do contato. (Os usuários e contatos que têm suas propriedades de gerente definidas para esse contato.) Somente leitura. Anulável. |
| manager | [directoryObject](directoryobject.md) | O usuário ou contato que é o gerente desse contato. Somente leitura. |
| memberOf | Coleção [directoryObject](directoryobject.md) | Grupos dos que esse contato é membro. Somente leitura. Anulável. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "directReports",
    "manager",
    "memberOf"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.orgContact"
}-->

``` json
{
  "addresses": [{"@odata.type": "microsoft.graph.physicalOfficeAddress"}],
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "jobTitle": "string",
  "mail": "string",
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "string (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSyncEnabled": true,
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "proxyAddresses": ["string"],
  "surname": "string"
}
```
