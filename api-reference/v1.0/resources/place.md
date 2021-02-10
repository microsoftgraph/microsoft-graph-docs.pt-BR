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
# <a name="place-resource-type"></a><span data-ttu-id="facbd-104">tipo de recurso place</span><span class="sxs-lookup"><span data-stu-id="facbd-104">place resource type</span></span>

<span data-ttu-id="facbd-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="facbd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="facbd-106">Representa atributos básicos de localização, como nome, endereço físico e coordenadas geográficas.</span><span class="sxs-lookup"><span data-stu-id="facbd-106">Represents basic location attributes such as name, physical address, and geographic coordinates.</span></span> <span data-ttu-id="facbd-107">Esse é o tipo base para tipos de localização mais ricos, [como sala](room.md) e [roomList](roomlist.md).</span><span class="sxs-lookup"><span data-stu-id="facbd-107">This is the base type for richer location types such as [room](room.md) and [roomList](roomlist.md).</span></span>

### <a name="using-the-places-api"></a><span data-ttu-id="facbd-108">Usando a API de locais</span><span class="sxs-lookup"><span data-stu-id="facbd-108">Using the places API</span></span>
<span data-ttu-id="facbd-109">Os administradores do Exchange Online podem organizar salas de reunião em um locatário em listas de salas.</span><span class="sxs-lookup"><span data-stu-id="facbd-109">Exchange Online administrators can organize meeting rooms in a tenant into room lists.</span></span> <span data-ttu-id="facbd-110">Usando a API de locais, você pode obter todas as listas de salas ou salas no locatário ou obter todas as salas em uma lista de salas específica.</span><span class="sxs-lookup"><span data-stu-id="facbd-110">Using the places API, you can get all the room lists or rooms in the tenant, or get all the rooms in a specific room list.</span></span>

<span data-ttu-id="facbd-111">Locais como [sala e](room.md) [roomList](roomlist.md) contêm a **ID** básica, o nome para exibição e o endereço de email.</span><span class="sxs-lookup"><span data-stu-id="facbd-111">Places like [room](room.md) and [roomList](roomlist.md) contain the basic **id**, display name and email address.</span></span> <span data-ttu-id="facbd-112">Além disso, eles contêm informações de navegação, como endereço físico e coordenadas geográficas, e no caso de salas, outras informações relevantes, como recursos de AV, número do piso e capacidade.</span><span class="sxs-lookup"><span data-stu-id="facbd-112">In addition, they contain navigational information like physical address and geographical coordinates, and in the case of rooms, other relevant information such as AV capabilities, floor number, and capacity.</span></span>

<span data-ttu-id="facbd-113">As [funções findRooms](/graph/api/user-findrooms) e [findRoomLists](/graph/api/user-findroomlists) suportam uma busca semelhante para salas e listas de salas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="facbd-113">The [findRooms](/graph/api/user-findrooms) and [findRoomLists](/graph/api/user-findroomlists) functions support similar lookup for rooms and room lists in a tenant.</span></span> <span data-ttu-id="facbd-114">A seguir está uma comparação entre a API de locais e essas funções.</span><span class="sxs-lookup"><span data-stu-id="facbd-114">The following is a comparison between the places API and these functions.</span></span>  <span data-ttu-id="facbd-115">Se você estiver criando um aplicativo de produção, escolha a API de locais, pois a API agora está geralmente disponível na v1.0.</span><span class="sxs-lookup"><span data-stu-id="facbd-115">If you are creating a production app, choose the places API as the API is now generally available in v1.0.</span></span> <span data-ttu-id="facbd-116">Planeje atualizar qualquer código existente que use **findRooms** ou **findRoomLists** para usar a API de locais, porque **findRooms** ou **findRoomLists** será preterido e uma linha do tempo será anunciada.</span><span class="sxs-lookup"><span data-stu-id="facbd-116">Plan to update any existing code that uses **findRooms** or **findRoomLists** to use the places API, because **findRooms** or **findRoomLists** will be deprecated, and a timeline will be announced.</span></span>

|<span data-ttu-id="facbd-117">Places API</span><span class="sxs-lookup"><span data-stu-id="facbd-117">Places API</span></span> |<span data-ttu-id="facbd-118">Funções findRooms e findRoomLists</span><span class="sxs-lookup"><span data-stu-id="facbd-118">findRooms and findRoomLists functions</span></span>|
|:------------------------------------|:-----------------------------|
|<span data-ttu-id="facbd-119">Oferece suporte para obter todas as salas ou listas de salas em um locatário e todas as salas em uma lista de salas</span><span class="sxs-lookup"><span data-stu-id="facbd-119">Supports getting all the rooms or room lists in a tenant, and all the rooms in a room list</span></span> | <span data-ttu-id="facbd-120">Suporte semelhante - obter todas as salas ou listas de salas em um locatário e todas as salas em uma lista de salas</span><span class="sxs-lookup"><span data-stu-id="facbd-120">Similar support - get all the rooms or room lists in a tenant, and all the rooms in a room list</span></span>|
|<span data-ttu-id="facbd-121">[Os locais de](../api/place-list.md) lista podem retornar mais de 100 salas em um locatário</span><span class="sxs-lookup"><span data-stu-id="facbd-121">[List places](../api/place-list.md) can return more than 100 rooms in a tenant</span></span> | <span data-ttu-id="facbd-122">[findRooms](/graph/api/user-findrooms) retorna até as primeiras 100 salas em um locatário</span><span class="sxs-lookup"><span data-stu-id="facbd-122">[findRooms](/graph/api/user-findrooms) returns up to the first 100 rooms in a tenant</span></span> |
|<span data-ttu-id="facbd-123">Dá [suporte a obter uma lista individual de sala ou sala](../api/place-get.md) em um locatário</span><span class="sxs-lookup"><span data-stu-id="facbd-123">Supports [getting an individual room or room list](../api/place-get.md) in a tenant</span></span> | <span data-ttu-id="facbd-124">Não dá suporte a obter uma lista individual de sala ou sala em um locatário</span><span class="sxs-lookup"><span data-stu-id="facbd-124">Does not support getting an individual room or room list in a tenant</span></span>
|<span data-ttu-id="facbd-125">Define as entidades específicas de [room](room.md) e [roomList](roomlist.md) que especificam um conjunto de propriedades mais rico, além do nome para exibição e endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="facbd-125">Defines the specific entities of [room](room.md) and [roomList](roomlist.md) which specify a richer property set, in addition to the display name and SMTP address.</span></span> | <span data-ttu-id="facbd-126">Cada sala e lista de sala é de um tipo [emailAddress](emailaddress.md) de peso mais claro que especifica apenas o nome de exibição e o endereço SMTP</span><span class="sxs-lookup"><span data-stu-id="facbd-126">Each room and room list is of a lighter weight [emailAddress](emailaddress.md) type which specifies only the display name and SMTP address</span></span>|
|<span data-ttu-id="facbd-127">Dá suporte somente a cenários organizacionais com permissões delegadas (contas de trabalho ou de estudante) ou permissões de aplicativo</span><span class="sxs-lookup"><span data-stu-id="facbd-127">Supports only organizational scenarios with delegated (work or school accounts) or application permissions</span></span> | <span data-ttu-id="facbd-128">Suporte semelhante apenas para cenários organizacionais com permissões delegadas ou de aplicativo</span><span class="sxs-lookup"><span data-stu-id="facbd-128">Similar support for only organizational scenarios with delegated or application permissions</span></span>|
|<span data-ttu-id="facbd-129">Dá [suporte à atualização de uma sala individual ou lista de sala](../api/place-update.md) em um locatário</span><span class="sxs-lookup"><span data-stu-id="facbd-129">Supports [updating an individual room or room list](../api/place-update.md) in a tenant</span></span> | <span data-ttu-id="facbd-130">Não dá suporte à atualização de uma lista individual de sala ou sala em um locatário</span><span class="sxs-lookup"><span data-stu-id="facbd-130">Does not support updating an individual room or room list in a tenant</span></span>

## <a name="methods"></a><span data-ttu-id="facbd-131">Métodos</span><span class="sxs-lookup"><span data-stu-id="facbd-131">Methods</span></span>

| <span data-ttu-id="facbd-132">Método</span><span class="sxs-lookup"><span data-stu-id="facbd-132">Method</span></span>                              | <span data-ttu-id="facbd-133">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="facbd-133">Return Type</span></span>                  | <span data-ttu-id="facbd-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="facbd-134">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="facbd-135">Listar locais</span><span class="sxs-lookup"><span data-stu-id="facbd-135">List places</span></span>](../api/place-list.md) | <span data-ttu-id="facbd-136">Uma coleção do tipo de local [](place.md) solicitado derivado</span><span class="sxs-lookup"><span data-stu-id="facbd-136">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="facbd-137">Obter uma coleção do tipo especificado de objetos **de local** definidos no locatário.</span><span class="sxs-lookup"><span data-stu-id="facbd-137">Get a collection of the specified type of **place** objects defined in the tenant.</span></span> |
| [<span data-ttu-id="facbd-138">Obter local</span><span class="sxs-lookup"><span data-stu-id="facbd-138">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="facbd-139">O tipo de local [](place.md) solicitado derivado</span><span class="sxs-lookup"><span data-stu-id="facbd-139">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="facbd-140">Obter as propriedades e os relacionamentos de um objeto **de local** especificado.</span><span class="sxs-lookup"><span data-stu-id="facbd-140">Get the properties and relationships of a specified **place** object.</span></span> |
| [<span data-ttu-id="facbd-141">Local de atualização</span><span class="sxs-lookup"><span data-stu-id="facbd-141">Update place</span></span>](../api/place-update.md)    | <span data-ttu-id="facbd-142">O tipo de local [](place.md) solicitado derivado</span><span class="sxs-lookup"><span data-stu-id="facbd-142">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="facbd-143">Atualize as propriedades e os relacionamentos de um objeto **de local** especificado.</span><span class="sxs-lookup"><span data-stu-id="facbd-143">Update the properties and relationships of a specified **place** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="facbd-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="facbd-144">Properties</span></span>

| <span data-ttu-id="facbd-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="facbd-145">Property</span></span>       | <span data-ttu-id="facbd-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="facbd-146">Type</span></span>                                              | <span data-ttu-id="facbd-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="facbd-147">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="facbd-148">address</span><span class="sxs-lookup"><span data-stu-id="facbd-148">address</span></span>        | [<span data-ttu-id="facbd-149">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="facbd-149">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="facbd-150">O endereço do local.</span><span class="sxs-lookup"><span data-stu-id="facbd-150">The street address of the place.</span></span> |
| <span data-ttu-id="facbd-151">displayName</span><span class="sxs-lookup"><span data-stu-id="facbd-151">displayName</span></span>    | <span data-ttu-id="facbd-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="facbd-152">String</span></span>                                            | <span data-ttu-id="facbd-153">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="facbd-153">The name associated with the place.</span></span> |
| <span data-ttu-id="facbd-154">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="facbd-154">geoCoordinates</span></span> | [<span data-ttu-id="facbd-155">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="facbd-155">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="facbd-156">Especifica o local em coordenadas de altitude de latitude, longitude e (opcionalmente).</span><span class="sxs-lookup"><span data-stu-id="facbd-156">Specifies the place location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="facbd-157">id</span><span class="sxs-lookup"><span data-stu-id="facbd-157">id</span></span>             | <span data-ttu-id="facbd-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="facbd-158">String</span></span>                                            | <span data-ttu-id="facbd-159">Identificador exclusivo do local.</span><span class="sxs-lookup"><span data-stu-id="facbd-159">Unique identifier for the place.</span></span> <span data-ttu-id="facbd-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="facbd-160">Read-only.</span></span> |
| <span data-ttu-id="facbd-161">phone</span><span class="sxs-lookup"><span data-stu-id="facbd-161">phone</span></span>          | <span data-ttu-id="facbd-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="facbd-162">String</span></span>                                            | <span data-ttu-id="facbd-163">O número de telefone do local.</span><span class="sxs-lookup"><span data-stu-id="facbd-163">The phone number of the place.</span></span> |

## <a name="relationships"></a><span data-ttu-id="facbd-164">Relações</span><span class="sxs-lookup"><span data-stu-id="facbd-164">Relationships</span></span>

<span data-ttu-id="facbd-165">Nenhum</span><span class="sxs-lookup"><span data-stu-id="facbd-165">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="facbd-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="facbd-166">JSON representation</span></span>

<span data-ttu-id="facbd-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="facbd-167">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="facbd-168">Confira também</span><span class="sxs-lookup"><span data-stu-id="facbd-168">See also</span></span>
- <span data-ttu-id="facbd-169">Para que os administradores criem uma lista de sala, use o cmdlet Do Exchange PowerShell [New-DistributionGroup](/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="facbd-169">For administrators to create a room list, use the Exchange PowerShell cmdlet [New-DistributionGroup](/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps).</span></span>
- <span data-ttu-id="facbd-170">Para que os administradores adicionem uma sala a uma lista de sala, use o cmdlet Do Exchange Powershell [Add-DistributionGroupMember](/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="facbd-170">For administrators to add a room to a room list, use the Exchange Powershell cmdlet [Add-DistributionGroupMember](/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps).</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
