---
title: tipo de recurso place
description: Representa um lugar. Esse é o tipo base para uma sala ou roomList.
ms.localizationpriority: medium
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8469be739bdf645e0d588af33918c5c51aecd3bf
ms.sourcegitcommit: 6a4e81d2b8e7447771c9060998c7e1cc18a57902
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/03/2022
ms.locfileid: "66609714"
---
# <a name="place-resource-type"></a>tipo de recurso place

Namespace: microsoft.graph

Representa atributos de localização básicos, como nome, endereço físico e coordenadas geográficas. Esse é o tipo base para tipos de localização mais avançados, como [room](room.md) e [roomList](roomlist.md).

### <a name="using-the-places-api"></a>Usando a API de locais
Exchange Online administradores podem organizar salas de reunião em um locatário em listas de salas. Usando a API de locais, você pode obter todas as listas de salas ou salas no locatário ou obter todas as salas em uma lista de salas específica.

Locais como [room e](room.md) [roomList](roomlist.md) contêm a **ID** básica, o nome de exibição e o endereço de email. Além disso, eles contêm informações de navegação, como endereço físico e coordenadas geográficas e, no caso de salas, outras informações relevantes, como recursos da AV, número de piso e capacidade.

As [funções findRooms](/graph/api/user-findrooms) e [findRoomLists](/graph/api/user-findroomlists) dão suporte a pesquisas semelhantes para salas e listas de salas em um locatário. A seguir está uma comparação entre a API de locais e essas funções.  Se você estiver criando um aplicativo de produção, escolha os locais da API, pois a API agora está em disponibilidade geral na v1.0. Planeje atualizar qualquer código existente que use **findRooms** ou **findRoomLists** para usar a API de locais, pois **findRooms** ou **findRoomLists** será preterido e uma linha do tempo será anunciada.

|API de Locais |Funções findRooms e findRoomLists|
|:------------------------------------|:-----------------------------|
|Dá suporte para obter todas as salas ou listas de salas em um locatário e todas as salas em uma lista de salas | Suporte semelhante – obtenha todas as salas ou listas de salas em um locatário e todas as salas em uma lista de salas|
|[Os locais de](../api/place-list.md) lista podem retornar mais de 100 salas em um locatário | [findRooms](/graph/api/user-findrooms) retorna até as primeiras 100 salas em um locatário |
|Dá [suporte a obter uma lista individual de sala ou sala](../api/place-get.md) em um locatário | Não dá suporte para obter uma lista individual de sala ou sala em um locatário
|Define as entidades específicas de [room](room.md) e [roomList](roomlist.md) que especificam um conjunto de propriedades mais avançado, além do nome de exibição e do endereço SMTP. | Cada lista de sala e sala é de um tipo [emailAddress](emailaddress.md) de peso mais leve que especifica apenas o nome de exibição e o endereço SMTP|
|Dá suporte apenas a cenários organizacionais com permissões delegadas (contas corporativas ou de estudante) ou de aplicativo | Suporte semelhante para apenas cenários organizacionais com permissões delegadas ou de aplicativo|
|Dá [suporte à atualização de uma lista de sala ou sala individual](../api/place-update.md) em um locatário | Não dá suporte à atualização de uma lista de sala ou sala individual em um locatário

## <a name="methods"></a>Métodos

| Método                              | Tipo de retorno                  | Descrição |
|:------------------------------------|:-----------------------------|:--------|
| [Listar locais](../api/place-list.md) | Uma coleção do tipo de local solicitado e [derivado](place.md) | Obtenha uma coleção do tipo especificado de objetos **de local** definidos no locatário. |
| [Obter local](../api/place-get.md)    | O tipo de local solicitado e [derivado](place.md)            | Obtenha as propriedades e as relações de um objeto **de local** especificado. |
| [Atualizar local](../api/place-update.md)    | O tipo de local solicitado e [derivado](place.md)            | Atualize as propriedades e as relações de um objeto **de local** especificado. |

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                                              | Descrição |
|:---------------|:--------------------------------------------------|:--------|
| address        | [physicalAddress](physicaladdress.md)             | O endereço do lugar. |
| displayName    | Cadeia de caracteres                                            | O nome associado ao local. |
| geoCoordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | Especifica o local do local nas coordenadas de latitude, longitude e altitude (opcionalmente). |
| id             | Cadeia de caracteres                                            | Identificador exclusivo do local. Somente leitura. |
| phone          | Cadeia de caracteres                                            | O número de telefone do lugar. |

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
- Para que os administradores criem uma lista de sala, use o cmdlet [New-DistributionGroup do Exchange PowerShell](/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps&preserve-view=true).
- Para que os administradores adicionem uma sala a uma lista de sala, use o cmdlet [Add-DistributionGroupMember do Exchange Powershell](/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps&preserve-view=true).

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
