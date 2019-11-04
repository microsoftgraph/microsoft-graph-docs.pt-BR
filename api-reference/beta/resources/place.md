---
title: inserir tipo de recurso
description: Representa um local. Este é o tipo base de uma sala ou sala de salas.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 975effa01ce60799a647bc051a0518d87afcda9e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939583"
---
# <a name="place-resource-type"></a><span data-ttu-id="2e68a-104">inserir tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="2e68a-104">place resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e68a-105">Representa os atributos de local básicos, como nome, endereço físico e coordenadas geográficas.</span><span class="sxs-lookup"><span data-stu-id="2e68a-105">Represents basic location attributes such as name, physical address, and geographic coordinates.</span></span> <span data-ttu-id="2e68a-106">Este é o tipo base para tipos de local mais avançados, como [sala](room.md) e [sala de salas](roomlist.md).</span><span class="sxs-lookup"><span data-stu-id="2e68a-106">This is the base type for richer location types such as [room](room.md) and [roomList](roomlist.md).</span></span>

### <a name="using-the-places-api"></a><span data-ttu-id="2e68a-107">Usando a API Places</span><span class="sxs-lookup"><span data-stu-id="2e68a-107">Using the places API</span></span>
<span data-ttu-id="2e68a-108">Os administradores do Exchange Online podem organizar as salas de reunião em um locatário em listas de salas.</span><span class="sxs-lookup"><span data-stu-id="2e68a-108">Exchange Online administrators can organize meeting rooms in a tenant into room lists.</span></span> <span data-ttu-id="2e68a-109">Usando a API de locais, você pode obter todas as listas de salas ou salas no locatário ou obter todas as salas em uma lista de salas específica.</span><span class="sxs-lookup"><span data-stu-id="2e68a-109">Using the places API, you can get all the room lists or rooms in the tenant, or get all the rooms in a specific room list.</span></span>

<span data-ttu-id="2e68a-110">Lugares como [sala](room.md) e [sala de salas](roomlist.md) contêm a **ID**básica, o nome para exibição e o endereço de email.</span><span class="sxs-lookup"><span data-stu-id="2e68a-110">Places like [room](room.md) and [roomList](roomlist.md) contain the basic **id**, display name and email address.</span></span> <span data-ttu-id="2e68a-111">Além disso, eles contêm informações de navegação, como endereço físico e coordenadas geográficas, e, no caso de salas, outras informações relevantes, como recursos AV, número de chão e capacidade.</span><span class="sxs-lookup"><span data-stu-id="2e68a-111">In addition, they contain navigational information like physical address and geographical coordinates, and in the case of rooms, other relevant information such as AV capabilities, floor number, and capacity.</span></span>

<span data-ttu-id="2e68a-112">As funções [findRooms](../api/user-findrooms.md) e [findRoomLists](../api/user-findroomlists.md) oferecem suporte à pesquisa semelhante para salas e listas de salas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="2e68a-112">The [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions support similar lookup for rooms and room lists in a tenant.</span></span> <span data-ttu-id="2e68a-113">Veja a seguir uma comparação entre a API de locais e essas funções.</span><span class="sxs-lookup"><span data-stu-id="2e68a-113">The following is a comparison between the places API and these functions.</span></span>

|<span data-ttu-id="2e68a-114">API de locais</span><span class="sxs-lookup"><span data-stu-id="2e68a-114">Places API</span></span> |<span data-ttu-id="2e68a-115">funções findRooms e findRoomLists</span><span class="sxs-lookup"><span data-stu-id="2e68a-115">findRooms and findRoomLists functions</span></span>|
|:------------------------------------|:-----------------------------|
|<span data-ttu-id="2e68a-116">Suporte para obter todas as listas de salas ou salas em um locatário e todas as salas em uma lista de salas</span><span class="sxs-lookup"><span data-stu-id="2e68a-116">Supports getting all the rooms or room lists in a tenant, and all the rooms in a room list</span></span> | <span data-ttu-id="2e68a-117">Suporte semelhante-obtenha todas as salas ou listas de salas em um locatário e todas as salas em uma lista de salas</span><span class="sxs-lookup"><span data-stu-id="2e68a-117">Similar support - get all the rooms or room lists in a tenant, and all the rooms in a room list</span></span>|
|<span data-ttu-id="2e68a-118">Os [locais de lista](../api/place-list.md) podem retornar mais de 100 salas em um locatário</span><span class="sxs-lookup"><span data-stu-id="2e68a-118">[List places](../api/place-list.md) can return more than 100 rooms in a tenant</span></span> | <span data-ttu-id="2e68a-119">[findRooms](../api/user-findrooms.md) retorna até as primeiras salas de 100 em um locatário</span><span class="sxs-lookup"><span data-stu-id="2e68a-119">[findRooms](../api/user-findrooms.md) returns up to the first 100 rooms in a tenant</span></span> |
|<span data-ttu-id="2e68a-120">Suporte para [obter uma lista de salas ou salas individuais](../api/place-get.md) em um locatário</span><span class="sxs-lookup"><span data-stu-id="2e68a-120">Supports [getting an individual room or room list](../api/place-get.md) in a tenant</span></span> | <span data-ttu-id="2e68a-121">Não oferece suporte para obter uma lista de salas ou salas individuais em um locatário</span><span class="sxs-lookup"><span data-stu-id="2e68a-121">Does not support getting an individual room or room list in a tenant</span></span>
|<span data-ttu-id="2e68a-122">Define as entidades específicas da [sala](room.md) e da [salalist](roomlist.md) que especificam um conjunto de propriedades mais avançado, além do nome para exibição e endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="2e68a-122">Defines the specific entities of [room](room.md) and [roomList](roomlist.md) which specify a richer property set, in addition to the display name and SMTP address.</span></span> | <span data-ttu-id="2e68a-123">Cada sala e lista de salas é de um tipo de endereço de email de espessura [mais leve que](emailaddress.md) especifica somente o nome para exibição e o endereço SMTP</span><span class="sxs-lookup"><span data-stu-id="2e68a-123">Each room and room list is of a lighter weight [emailAddress](emailaddress.md) type which specifies only the display name and SMTP address</span></span>|
|<span data-ttu-id="2e68a-124">Oferece suporte somente a cenários organizacionais com permissões delegadas (contas corporativas ou de estudante) ou de aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e68a-124">Supports only organizational scenarios with delegated (work or school accounts) or application permissions</span></span> | <span data-ttu-id="2e68a-125">Suporte semelhante somente para cenários organizacionais com permissões delegadas ou de aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e68a-125">Similar support for only organizational scenarios with delegated or application permissions</span></span>|
|<span data-ttu-id="2e68a-126">Oferece suporte à [atualização de uma lista de salas ou salas individuais](../api/place-update.md) em um locatário</span><span class="sxs-lookup"><span data-stu-id="2e68a-126">Supports [updating an individual room or room list](../api/place-update.md) in a tenant</span></span> | <span data-ttu-id="2e68a-127">Não oferece suporte à atualização de uma lista de salas ou salas individuais em um locatário</span><span class="sxs-lookup"><span data-stu-id="2e68a-127">Does not support updating an individual room or room list in a tenant</span></span>

## <a name="methods"></a><span data-ttu-id="2e68a-128">Métodos</span><span class="sxs-lookup"><span data-stu-id="2e68a-128">Methods</span></span>

| <span data-ttu-id="2e68a-129">Método</span><span class="sxs-lookup"><span data-stu-id="2e68a-129">Method</span></span>                              | <span data-ttu-id="2e68a-130">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2e68a-130">Return Type</span></span>                  | <span data-ttu-id="2e68a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e68a-131">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="2e68a-132">Locais de lista</span><span class="sxs-lookup"><span data-stu-id="2e68a-132">List places</span></span>](../api/place-list.md) | <span data-ttu-id="2e68a-133">Uma coleção do tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="2e68a-133">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="2e68a-134">Obtém uma coleção do tipo especificado de objetos **Place** definidos no locatário.</span><span class="sxs-lookup"><span data-stu-id="2e68a-134">Get a collection of the specified type of **place** objects defined in the tenant.</span></span> |
| [<span data-ttu-id="2e68a-135">Obter local</span><span class="sxs-lookup"><span data-stu-id="2e68a-135">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="2e68a-136">O tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="2e68a-136">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="2e68a-137">Obtenha as propriedades e os relacionamentos de um objeto **local** especificado.</span><span class="sxs-lookup"><span data-stu-id="2e68a-137">Get the properties and relationships of a specified **place** object.</span></span> |
| [<span data-ttu-id="2e68a-138">Local de atualização</span><span class="sxs-lookup"><span data-stu-id="2e68a-138">Update place</span></span>](../api/place-update.md)    | <span data-ttu-id="2e68a-139">O tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="2e68a-139">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="2e68a-140">Atualizar as propriedades e os relacionamentos de um objeto **local** especificado.</span><span class="sxs-lookup"><span data-stu-id="2e68a-140">Update the properties and relationships of a specified **place** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2e68a-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2e68a-141">Properties</span></span>

| <span data-ttu-id="2e68a-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e68a-142">Property</span></span>       | <span data-ttu-id="2e68a-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e68a-143">Type</span></span>                                              | <span data-ttu-id="2e68a-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e68a-144">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="2e68a-145">address</span><span class="sxs-lookup"><span data-stu-id="2e68a-145">address</span></span>        | [<span data-ttu-id="2e68a-146">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="2e68a-146">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="2e68a-147">O endereço da rua do local.</span><span class="sxs-lookup"><span data-stu-id="2e68a-147">The street address of the place.</span></span> |
| <span data-ttu-id="2e68a-148">displayName</span><span class="sxs-lookup"><span data-stu-id="2e68a-148">displayName</span></span>    | <span data-ttu-id="2e68a-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e68a-149">String</span></span>                                            | <span data-ttu-id="2e68a-150">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="2e68a-150">The name associated with the place.</span></span> |
| <span data-ttu-id="2e68a-151">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="2e68a-151">geoCoordinates</span></span> | [<span data-ttu-id="2e68a-152">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="2e68a-152">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="2e68a-153">Especifica o local do local no latitude, longitude e (opcionalmente) as coordenadas de altitude.</span><span class="sxs-lookup"><span data-stu-id="2e68a-153">Specifies the place location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="2e68a-154">id</span><span class="sxs-lookup"><span data-stu-id="2e68a-154">id</span></span>             | <span data-ttu-id="2e68a-155">String</span><span class="sxs-lookup"><span data-stu-id="2e68a-155">String</span></span>                                            | <span data-ttu-id="2e68a-156">Identificador exclusivo do local.</span><span class="sxs-lookup"><span data-stu-id="2e68a-156">Unique identifier for the place.</span></span> <span data-ttu-id="2e68a-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e68a-157">Read-only.</span></span> |
| <span data-ttu-id="2e68a-158">phone</span><span class="sxs-lookup"><span data-stu-id="2e68a-158">phone</span></span>          | <span data-ttu-id="2e68a-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e68a-159">String</span></span>                                            | <span data-ttu-id="2e68a-160">O número de telefone do local.</span><span class="sxs-lookup"><span data-stu-id="2e68a-160">The phone number of the place.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2e68a-161">Relações</span><span class="sxs-lookup"><span data-stu-id="2e68a-161">Relationships</span></span>

<span data-ttu-id="2e68a-162">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e68a-162">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e68a-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2e68a-163">JSON representation</span></span>

<span data-ttu-id="2e68a-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2e68a-164">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="2e68a-165">Confira também</span><span class="sxs-lookup"><span data-stu-id="2e68a-165">See also</span></span>
- <span data-ttu-id="2e68a-166">Para que os administradores criem uma lista de salas, use o [novo](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps)grupo de distribuição do cmdlet do Exchange PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2e68a-166">For administrators to create a room list, use the Exchange PowerShell cmdlet [New-DistributionGroup](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps).</span></span>
- <span data-ttu-id="2e68a-167">Para que os administradores adicionem uma sala a uma lista de salas, use o cmdlet do Exchange PowerShell [Add-DistributionGroupMember](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="2e68a-167">For administrators to add a room to a room list, use the Exchange Powershell cmdlet [Add-DistributionGroupMember](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps).</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
