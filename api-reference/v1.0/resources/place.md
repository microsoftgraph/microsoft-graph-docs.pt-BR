---
title: inserir tipo de recurso
description: Representa um local. Este é o tipo base de uma sala ou sala de salas.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d7554463870556791f7f422928c17aa25819ebc8
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581712"
---
# <a name="place-resource-type"></a><span data-ttu-id="6b381-104">inserir tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="6b381-104">place resource type</span></span>

<span data-ttu-id="6b381-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b381-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b381-106">Representa os atributos de local básicos, como nome, endereço físico e coordenadas geográficas.</span><span class="sxs-lookup"><span data-stu-id="6b381-106">Represents basic location attributes such as name, physical address, and geographic coordinates.</span></span> <span data-ttu-id="6b381-107">Este é o tipo base para tipos de local mais avançados, como [sala](room.md) e [sala de salas](roomlist.md).</span><span class="sxs-lookup"><span data-stu-id="6b381-107">This is the base type for richer location types such as [room](room.md) and [roomList](roomlist.md).</span></span>

### <a name="using-the-places-api"></a><span data-ttu-id="6b381-108">Usando a API Places</span><span class="sxs-lookup"><span data-stu-id="6b381-108">Using the places API</span></span>
<span data-ttu-id="6b381-109">Os administradores do Exchange Online podem organizar as salas de reunião em um locatário em listas de salas.</span><span class="sxs-lookup"><span data-stu-id="6b381-109">Exchange Online administrators can organize meeting rooms in a tenant into room lists.</span></span> <span data-ttu-id="6b381-110">Usando a API de locais, você pode obter todas as listas de salas ou salas no locatário ou obter todas as salas em uma lista de salas específica.</span><span class="sxs-lookup"><span data-stu-id="6b381-110">Using the places API, you can get all the room lists or rooms in the tenant, or get all the rooms in a specific room list.</span></span>

<span data-ttu-id="6b381-111">Lugares como [sala](room.md) e [sala de salas](roomlist.md) contêm a **ID**básica, o nome para exibição e o endereço de email.</span><span class="sxs-lookup"><span data-stu-id="6b381-111">Places like [room](room.md) and [roomList](roomlist.md) contain the basic **id**, display name and email address.</span></span> <span data-ttu-id="6b381-112">Além disso, eles contêm informações de navegação, como endereço físico e coordenadas geográficas, e, no caso de salas, outras informações relevantes, como recursos AV, número de chão e capacidade.</span><span class="sxs-lookup"><span data-stu-id="6b381-112">In addition, they contain navigational information like physical address and geographical coordinates, and in the case of rooms, other relevant information such as AV capabilities, floor number, and capacity.</span></span>

<span data-ttu-id="6b381-113">As funções [findRooms](/graph/api/user-findrooms) e [findRoomLists](/graph/api/user-findroomlists) oferecem suporte à pesquisa semelhante para salas e listas de salas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="6b381-113">The [findRooms](/graph/api/user-findrooms) and [findRoomLists](/graph/api/user-findroomlists) functions support similar lookup for rooms and room lists in a tenant.</span></span> <span data-ttu-id="6b381-114">Veja a seguir uma comparação entre a API de locais e essas funções.</span><span class="sxs-lookup"><span data-stu-id="6b381-114">The following is a comparison between the places API and these functions.</span></span>  <span data-ttu-id="6b381-115">Se você estiver criando um aplicativo de produção, escolha a API de lugares como a API está agora disponível em v 1.0.</span><span class="sxs-lookup"><span data-stu-id="6b381-115">If you are creating a production app, choose the places API as the API is now generally available in v1.0.</span></span> <span data-ttu-id="6b381-116">Planeje a atualização de qualquer código existente que use o **findRooms** ou o **findRoomLists** para usar a API de locais, pois o **findRooms** ou o **findRoomLists** será preterido e uma linha do tempo será anunciada.</span><span class="sxs-lookup"><span data-stu-id="6b381-116">Plan to update any existing code that uses **findRooms** or **findRoomLists** to use the places API, because **findRooms** or **findRoomLists** will be deprecated, and a timeline will be announced.</span></span>

|<span data-ttu-id="6b381-117">API de locais</span><span class="sxs-lookup"><span data-stu-id="6b381-117">Places API</span></span> |<span data-ttu-id="6b381-118">funções findRooms e findRoomLists</span><span class="sxs-lookup"><span data-stu-id="6b381-118">findRooms and findRoomLists functions</span></span>|
|:------------------------------------|:-----------------------------|
|<span data-ttu-id="6b381-119">Suporte para obter todas as listas de salas ou salas em um locatário e todas as salas em uma lista de salas</span><span class="sxs-lookup"><span data-stu-id="6b381-119">Supports getting all the rooms or room lists in a tenant, and all the rooms in a room list</span></span> | <span data-ttu-id="6b381-120">Suporte semelhante-obtenha todas as salas ou listas de salas em um locatário e todas as salas em uma lista de salas</span><span class="sxs-lookup"><span data-stu-id="6b381-120">Similar support - get all the rooms or room lists in a tenant, and all the rooms in a room list</span></span>|
|<span data-ttu-id="6b381-121">Os [locais de lista](../api/place-list.md) podem retornar mais de 100 salas em um locatário</span><span class="sxs-lookup"><span data-stu-id="6b381-121">[List places](../api/place-list.md) can return more than 100 rooms in a tenant</span></span> | <span data-ttu-id="6b381-122">[findRooms](/graph/api/user-findrooms) retorna até as primeiras salas de 100 em um locatário</span><span class="sxs-lookup"><span data-stu-id="6b381-122">[findRooms](/graph/api/user-findrooms) returns up to the first 100 rooms in a tenant</span></span> |
|<span data-ttu-id="6b381-123">Suporte para [obter uma lista de salas ou salas individuais](../api/place-get.md) em um locatário</span><span class="sxs-lookup"><span data-stu-id="6b381-123">Supports [getting an individual room or room list](../api/place-get.md) in a tenant</span></span> | <span data-ttu-id="6b381-124">Não oferece suporte para obter uma lista de salas ou salas individuais em um locatário</span><span class="sxs-lookup"><span data-stu-id="6b381-124">Does not support getting an individual room or room list in a tenant</span></span>
|<span data-ttu-id="6b381-125">Define as entidades específicas da [sala](room.md) e da [salalist](roomlist.md) que especificam um conjunto de propriedades mais avançado, além do nome para exibição e endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="6b381-125">Defines the specific entities of [room](room.md) and [roomList](roomlist.md) which specify a richer property set, in addition to the display name and SMTP address.</span></span> | <span data-ttu-id="6b381-126">Cada sala e lista de salas é de um tipo de endereço de email de espessura [mais leve que](emailaddress.md) especifica somente o nome para exibição e o endereço SMTP</span><span class="sxs-lookup"><span data-stu-id="6b381-126">Each room and room list is of a lighter weight [emailAddress](emailaddress.md) type which specifies only the display name and SMTP address</span></span>|
|<span data-ttu-id="6b381-127">Oferece suporte somente a cenários organizacionais com permissões delegadas (contas corporativas ou de estudante) ou de aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b381-127">Supports only organizational scenarios with delegated (work or school accounts) or application permissions</span></span> | <span data-ttu-id="6b381-128">Suporte semelhante somente para cenários organizacionais com permissões delegadas ou de aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b381-128">Similar support for only organizational scenarios with delegated or application permissions</span></span>|
|<span data-ttu-id="6b381-129">Oferece suporte à [atualização de uma lista de salas ou salas individuais](../api/place-update.md) em um locatário</span><span class="sxs-lookup"><span data-stu-id="6b381-129">Supports [updating an individual room or room list](../api/place-update.md) in a tenant</span></span> | <span data-ttu-id="6b381-130">Não oferece suporte à atualização de uma lista de salas ou salas individuais em um locatário</span><span class="sxs-lookup"><span data-stu-id="6b381-130">Does not support updating an individual room or room list in a tenant</span></span>

## <a name="methods"></a><span data-ttu-id="6b381-131">Methods</span><span class="sxs-lookup"><span data-stu-id="6b381-131">Methods</span></span>

| <span data-ttu-id="6b381-132">Método</span><span class="sxs-lookup"><span data-stu-id="6b381-132">Method</span></span>                              | <span data-ttu-id="6b381-133">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6b381-133">Return Type</span></span>                  | <span data-ttu-id="6b381-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b381-134">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="6b381-135">Locais de lista</span><span class="sxs-lookup"><span data-stu-id="6b381-135">List places</span></span>](../api/place-list.md) | <span data-ttu-id="6b381-136">Uma coleção do tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="6b381-136">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="6b381-137">Obtém uma coleção do tipo especificado de objetos **Place** definidos no locatário.</span><span class="sxs-lookup"><span data-stu-id="6b381-137">Get a collection of the specified type of **place** objects defined in the tenant.</span></span> |
| [<span data-ttu-id="6b381-138">Obter local</span><span class="sxs-lookup"><span data-stu-id="6b381-138">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="6b381-139">O tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="6b381-139">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="6b381-140">Obtenha as propriedades e os relacionamentos de um objeto **local** especificado.</span><span class="sxs-lookup"><span data-stu-id="6b381-140">Get the properties and relationships of a specified **place** object.</span></span> |
| [<span data-ttu-id="6b381-141">Local de atualização</span><span class="sxs-lookup"><span data-stu-id="6b381-141">Update place</span></span>](../api/place-update.md)    | <span data-ttu-id="6b381-142">O tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="6b381-142">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="6b381-143">Atualizar as propriedades e os relacionamentos de um objeto **local** especificado.</span><span class="sxs-lookup"><span data-stu-id="6b381-143">Update the properties and relationships of a specified **place** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6b381-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b381-144">Properties</span></span>

| <span data-ttu-id="6b381-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b381-145">Property</span></span>       | <span data-ttu-id="6b381-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b381-146">Type</span></span>                                              | <span data-ttu-id="6b381-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b381-147">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="6b381-148">address</span><span class="sxs-lookup"><span data-stu-id="6b381-148">address</span></span>        | [<span data-ttu-id="6b381-149">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="6b381-149">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="6b381-150">O endereço da rua do local.</span><span class="sxs-lookup"><span data-stu-id="6b381-150">The street address of the place.</span></span> |
| <span data-ttu-id="6b381-151">displayName</span><span class="sxs-lookup"><span data-stu-id="6b381-151">displayName</span></span>    | <span data-ttu-id="6b381-152">String</span><span class="sxs-lookup"><span data-stu-id="6b381-152">String</span></span>                                            | <span data-ttu-id="6b381-153">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="6b381-153">The name associated with the place.</span></span> |
| <span data-ttu-id="6b381-154">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="6b381-154">geoCoordinates</span></span> | [<span data-ttu-id="6b381-155">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="6b381-155">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="6b381-156">Especifica o local do local no latitude, longitude e (opcionalmente) as coordenadas de altitude.</span><span class="sxs-lookup"><span data-stu-id="6b381-156">Specifies the place location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="6b381-157">id</span><span class="sxs-lookup"><span data-stu-id="6b381-157">id</span></span>             | <span data-ttu-id="6b381-158">String</span><span class="sxs-lookup"><span data-stu-id="6b381-158">String</span></span>                                            | <span data-ttu-id="6b381-159">Identificador exclusivo do local.</span><span class="sxs-lookup"><span data-stu-id="6b381-159">Unique identifier for the place.</span></span> <span data-ttu-id="6b381-160">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="6b381-160">Read-only.</span></span> |
| <span data-ttu-id="6b381-161">phone</span><span class="sxs-lookup"><span data-stu-id="6b381-161">phone</span></span>          | <span data-ttu-id="6b381-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b381-162">String</span></span>                                            | <span data-ttu-id="6b381-163">O número de telefone do local.</span><span class="sxs-lookup"><span data-stu-id="6b381-163">The phone number of the place.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6b381-164">Relações</span><span class="sxs-lookup"><span data-stu-id="6b381-164">Relationships</span></span>

<span data-ttu-id="6b381-165">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b381-165">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b381-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b381-166">JSON representation</span></span>

<span data-ttu-id="6b381-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b381-167">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="6b381-168">Confira também</span><span class="sxs-lookup"><span data-stu-id="6b381-168">See also</span></span>
- <span data-ttu-id="6b381-169">Para que os administradores criem uma lista de salas, use o [novo](/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps)grupo de distribuição do cmdlet do Exchange PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6b381-169">For administrators to create a room list, use the Exchange PowerShell cmdlet [New-DistributionGroup](/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps).</span></span>
- <span data-ttu-id="6b381-170">Para que os administradores adicionem uma sala a uma lista de salas, use o cmdlet do Exchange PowerShell [Add-DistributionGroupMember](/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="6b381-170">For administrators to add a room to a room list, use the Exchange Powershell cmdlet [Add-DistributionGroupMember](/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps).</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
