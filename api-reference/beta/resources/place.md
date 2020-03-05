---
title: inserir tipo de recurso
description: Representa um local. Este é o tipo base de uma sala ou sala de salas.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ea1736e0215b411673f8c458f79c57181312a25a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521839"
---
# <a name="place-resource-type"></a>inserir tipo de recurso

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os atributos de local básicos, como nome, endereço físico e coordenadas geográficas. Este é o tipo base para tipos de local mais avançados, como [sala](room.md) e [sala de salas](roomlist.md).

### <a name="using-the-places-api"></a>Usando a API Places
Os administradores do Exchange Online podem organizar as salas de reunião em um locatário em listas de salas. Usando a API de locais, você pode obter todas as listas de salas ou salas no locatário ou obter todas as salas em uma lista de salas específica.

Lugares como [sala](room.md) e [sala de salas](roomlist.md) contêm a **ID**básica, o nome para exibição e o endereço de email. Além disso, eles contêm informações de navegação, como endereço físico e coordenadas geográficas, e, no caso de salas, outras informações relevantes, como recursos AV, número de chão e capacidade.

As funções [findRooms](../api/user-findrooms.md) e [findRoomLists](../api/user-findroomlists.md) oferecem suporte à pesquisa semelhante para salas e listas de salas em um locatário. Veja a seguir uma comparação entre a API de locais e essas funções.

|API de locais |funções findRooms e findRoomLists|
|:------------------------------------|:-----------------------------|
|Suporte para obter todas as listas de salas ou salas em um locatário e todas as salas em uma lista de salas | Suporte semelhante-obtenha todas as salas ou listas de salas em um locatário e todas as salas em uma lista de salas|
|Os [locais de lista](../api/place-list.md) podem retornar mais de 100 salas em um locatário | [findRooms](../api/user-findrooms.md) retorna até as primeiras salas de 100 em um locatário |
|Suporte para [obter uma lista de salas ou salas individuais](../api/place-get.md) em um locatário | Não oferece suporte para obter uma lista de salas ou salas individuais em um locatário
|Define as entidades específicas da [sala](room.md) e da [salalist](roomlist.md) que especificam um conjunto de propriedades mais avançado, além do nome para exibição e endereço SMTP. | Cada sala e lista de salas é de um tipo de endereço de email de espessura [mais leve que](emailaddress.md) especifica somente o nome para exibição e o endereço SMTP|
|Oferece suporte somente a cenários organizacionais com permissões delegadas (contas corporativas ou de estudante) ou de aplicativo | Suporte semelhante somente para cenários organizacionais com permissões delegadas ou de aplicativo|
|Oferece suporte à [atualização de uma lista de salas ou salas individuais](../api/place-update.md) em um locatário | Não oferece suporte à atualização de uma lista de salas ou salas individuais em um locatário

## <a name="methods"></a>Métodos

| Método                              | Tipo de retorno                  | Descrição |
|:------------------------------------|:-----------------------------|:--------|
| [Locais de lista](../api/place-list.md) | Uma coleção do tipo de [local](place.md) solicitado e derivado | Obtém uma coleção do tipo especificado de objetos **Place** definidos no locatário. |
| [Obter local](../api/place-get.md)    | O tipo de [local](place.md) solicitado e derivado            | Obtenha as propriedades e os relacionamentos de um objeto **local** especificado. |
| [Local de atualização](../api/place-update.md)    | O tipo de [local](place.md) solicitado e derivado            | Atualizar as propriedades e os relacionamentos de um objeto **local** especificado. |

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                                              | Descrição |
|:---------------|:--------------------------------------------------|:--------|
| address        | [physicalAddress](physicaladdress.md)             | O endereço da rua do local. |
| displayName    | Cadeia de caracteres                                            | O nome associado ao local. |
| geoCoordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | Especifica o local do local no latitude, longitude e (opcionalmente) as coordenadas de altitude. |
| id             | String                                            | Identificador exclusivo do local. Somente leitura. |
| phone          | Cadeia de caracteres                                            | O número de telefone do local. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.place",
  "baseType": ""
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
- Para que os administradores criem uma lista de salas, use o [novo](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps)grupo de distribuição do cmdlet do Exchange PowerShell.
- Para que os administradores adicionem uma sala a uma lista de salas, use o cmdlet do Exchange PowerShell [Add-DistributionGroupMember](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps).

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
