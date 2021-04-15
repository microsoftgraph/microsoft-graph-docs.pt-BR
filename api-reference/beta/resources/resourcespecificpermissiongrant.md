---
title: tipo de recurso resourceSpecificPermissionGrant
description: Especifica a permissão que um aplicativo específico do Azure AD tem.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7119d25f25b0e4f382a077ca6a1264dc22e11d5b
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51765899"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="798fd-103">tipo de recurso resourceSpecificPermissionGrant</span><span class="sxs-lookup"><span data-stu-id="798fd-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="798fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="798fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="798fd-105">Um resourceSpecificPermissionGrant declara a permissão concedida a um aplicativo específico do AzureAD para uma instância de um recurso no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="798fd-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="798fd-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="798fd-106">Methods</span></span>

|  <span data-ttu-id="798fd-107">Método</span><span class="sxs-lookup"><span data-stu-id="798fd-107">Method</span></span>                                                                   |  <span data-ttu-id="798fd-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="798fd-108">Return Type</span></span>                                                                     | <span data-ttu-id="798fd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="798fd-109">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="798fd-110">Listar concessões de permissão de um chat</span><span class="sxs-lookup"><span data-stu-id="798fd-110">List permission grants of a chat</span></span>](../api/chat-list-permissiongrants.md)   | <span data-ttu-id="798fd-111">[coleção resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="798fd-111">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="798fd-112">Listar permissões concedidas em um chat específico.</span><span class="sxs-lookup"><span data-stu-id="798fd-112">List permissions that have been granted in a specific chat.</span></span>  |
|[<span data-ttu-id="798fd-113">Listar concessões de permissão de um grupo</span><span class="sxs-lookup"><span data-stu-id="798fd-113">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="798fd-114">[coleção resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="798fd-114">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="798fd-115">Listar permissões concedidas em um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="798fd-115">List permissions that have been granted in a specific group.</span></span> |

## <a name="properties"></a><span data-ttu-id="798fd-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="798fd-116">Properties</span></span>

| <span data-ttu-id="798fd-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="798fd-117">Property</span></span>        | <span data-ttu-id="798fd-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="798fd-118">Type</span></span>          | <span data-ttu-id="798fd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="798fd-119">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="798fd-120">id</span><span class="sxs-lookup"><span data-stu-id="798fd-120">id</span></span>              | <span data-ttu-id="798fd-121">string</span><span class="sxs-lookup"><span data-stu-id="798fd-121">string</span></span>        | <span data-ttu-id="798fd-122">O identificador exclusivo da concessão de permissão específica do recurso.</span><span class="sxs-lookup"><span data-stu-id="798fd-122">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="798fd-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="798fd-123">Read-only.</span></span>           |
| <span data-ttu-id="798fd-124">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="798fd-124">deletedDateTime</span></span> | <span data-ttu-id="798fd-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="798fd-125">dateTimeOffset</span></span>| <span data-ttu-id="798fd-126">Não usado.</span><span class="sxs-lookup"><span data-stu-id="798fd-126">Not used.</span></span>                                                                             |
| <span data-ttu-id="798fd-127">clientId</span><span class="sxs-lookup"><span data-stu-id="798fd-127">clientId</span></span>        | <span data-ttu-id="798fd-128">string</span><span class="sxs-lookup"><span data-stu-id="798fd-128">string</span></span>        | <span data-ttu-id="798fd-129">ID do aplicativo do Azure AD que recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="798fd-129">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="798fd-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="798fd-130">Read-only.</span></span>                            |
| <span data-ttu-id="798fd-131">clientAppId</span><span class="sxs-lookup"><span data-stu-id="798fd-131">clientAppId</span></span>     | <span data-ttu-id="798fd-132">string</span><span class="sxs-lookup"><span data-stu-id="798fd-132">string</span></span>        | <span data-ttu-id="798fd-133">ID da entidade de serviço do aplicativo do Azure AD que recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="798fd-133">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="798fd-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="798fd-134">Read-only.</span></span>   |
| <span data-ttu-id="798fd-135">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="798fd-135">resourceAppId</span></span>   | <span data-ttu-id="798fd-136">string</span><span class="sxs-lookup"><span data-stu-id="798fd-136">string</span></span>        | <span data-ttu-id="798fd-137">ID do aplicativo do Azure AD que está hospedando o recurso.</span><span class="sxs-lookup"><span data-stu-id="798fd-137">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="798fd-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="798fd-138">Read-only.</span></span>                        |
| <span data-ttu-id="798fd-139">permissionType</span><span class="sxs-lookup"><span data-stu-id="798fd-139">permissionType</span></span>  | <span data-ttu-id="798fd-140">string</span><span class="sxs-lookup"><span data-stu-id="798fd-140">string</span></span>        | <span data-ttu-id="798fd-141">O tipo de permissão.</span><span class="sxs-lookup"><span data-stu-id="798fd-141">The type of permission.</span></span> <span data-ttu-id="798fd-142">Os valores possíveis são: `Application` e `Delegated`.</span><span class="sxs-lookup"><span data-stu-id="798fd-142">Possible values are: `Application`, `Delegated`.</span></span> <span data-ttu-id="798fd-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="798fd-143">Read-only.</span></span> |
| <span data-ttu-id="798fd-144">permission</span><span class="sxs-lookup"><span data-stu-id="798fd-144">permission</span></span>      | <span data-ttu-id="798fd-145">string</span><span class="sxs-lookup"><span data-stu-id="798fd-145">string</span></span>        | <span data-ttu-id="798fd-146">O nome da permissão.</span><span class="sxs-lookup"><span data-stu-id="798fd-146">The name of the permission.</span></span> <span data-ttu-id="798fd-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="798fd-147">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="798fd-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="798fd-148">JSON representation</span></span>

<span data-ttu-id="798fd-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="798fd-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant"
}-->

```json
{
  "id": "string (identifier)",
  "deletedDateTime": "dateTimeOffset",
  "clientId": "string",
  "clientAppId": "string",
  "resourceAppId": "string",
  "permissionType": "string",
  "permission": "string"
}
```


