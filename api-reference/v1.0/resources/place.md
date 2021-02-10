---
title: tipo de recurso place
description: Representa um local. Esse é o tipo de base para uma sala ou roomList.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0897cf9105ae0260803fa81291ab879bd7876b86
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156340"
---
# <a name="place-resource-type"></a>tipo de recurso place

Namespace: microsoft.graph

Representa atributos básicos de localização, como nome, endereço físico e coordenadas geográficas. Esse é o tipo base para tipos de localização mais ricos, [como sala](room.md) e [roomList](roomlist.md).

### <a name="using-the-places-api"></a>Usando a API de locais
Os administradores do Exchange Online podem organizar salas de reunião em um locatário em listas de salas. Usando a API de locais, você pode obter todas as listas de salas ou salas no locatário ou obter todas as salas em uma lista de salas específica.

Locais como [sala e](room.md) [roomList](roomlist.md) contêm a **ID** básica, o nome para exibição e o endereço de email. Além disso, eles contêm informações de navegação, como endereço físico e coordenadas geográficas, e no caso de salas, outras informações relevantes, como recursos de AV, número do piso e capacidade.

As [funções findRooms](/graph/api/user-findrooms) e [findRoomLists](/graph/api/user-findroomlists) suportam uma busca semelhante para salas e listas de salas em um locatário. A seguir está uma comparação entre a API de locais e essas funções.  Se você estiver criando um aplicativo de produção, escolha a API de locais, pois a API agora está geralmente disponível na v1.0. Planeje atualizar qualquer código existente que use **findRooms** ou **findRoomLists** para usar a API de locais, porque **findRooms** ou **findRoomLists** será preterido e uma linha do tempo será anunciada.

|Places API |Funções findRooms e findRoomLists|
|:------------------------------------|:-----------------------------|
|Oferece suporte para obter todas as salas ou listas de salas em um locatário e todas as salas em uma lista de salas | Suporte semelhante - obter todas as salas ou listas de salas em um locatário e todas as salas em uma lista de salas|
|[Os locais de](../api/place-list.md) lista podem retornar mais de 100 salas em um locatário | [findRooms](/graph/api/user-findrooms) retorna até as primeiras 100 salas em um locatário |
|Dá [suporte a obter uma lista individual de sala ou sala](../api/place-get.md) em um locatário | Não dá suporte a obter uma lista individual de sala ou sala em um locatário
|Define as entidades específicas de [room](room.md) e [roomList](roomlist.md) que especificam um conjunto de propriedades mais rico, além do nome para exibição e endereço SMTP. | Cada sala e lista de sala é de um tipo [emailAddress](emailaddress.md) de peso mais claro que especifica apenas o nome de exibição e o endereço SMTP|
|Dá suporte somente a cenários organizacionais com permissões delegadas (contas de trabalho ou de estudante) ou permissões de aplicativo | Suporte semelhante apenas para cenários organizacionais com permissões delegadas ou de aplicativo|
|Dá [suporte à atualização de uma sala individual ou lista de sala](../api/place-update.md) em um locatário | Não dá suporte à atualização de uma lista individual de sala ou sala em um locatário

## <a name="methods"></a>Métodos

| Método                              | Tipo de retorno                  | Descrição |
|:------------------------------------|:-----------------------------|:--------|
| [Listar locais](../api/place-list.md) | Uma coleção do tipo de local [](place.md) solicitado derivado | Obter uma coleção do tipo especificado de objetos **de local** definidos no locatário. |
| [Obter local](../api/place-get.md)    | O tipo de local [](place.md) solicitado derivado            | Obter as propriedades e os relacionamentos de um objeto **de local** especificado. |
| [Local de atualização](../api/place-update.md)    | O tipo de local [](place.md) solicitado derivado            | Atualize as propriedades e os relacionamentos de um objeto **de local** especificado. |

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                                              | Descrição |
|:---------------|:--------------------------------------------------|:--------|
| address        | [physicalAddress](physicaladdress.md)             | O endereço do local. |
| displayName    | Cadeia de caracteres                                            | O nome associado ao local. |
| geoCoordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | Especifica o local em coordenadas de altitude de latitude, longitude e (opcionalmente). |
| id             | Cadeia de caracteres                                            | Identificador exclusivo do local. Somente leitura. |
| phone          | Cadeia de caracteres                                            | O número de telefone do local. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.place"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "String",
  "id": "String (identifier)",
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "phone": "String"
}
```

## <a name="see-also"></a>Confira também
- Para que os administradores criem uma lista de sala, use o cmdlet Do Exchange PowerShell [New-DistributionGroup](/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps).
- Para que os administradores adicionem uma sala a uma lista de sala, use o cmdlet Do Exchange Powershell [Add-DistributionGroupMember](/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps).

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
