---
title: tipo de recurso resourceSpecificPermissionGrant
description: Especifica a permissão que um aplicativo específico do Azure AD tem.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 56d7ea203f4ed72f45a3650197c1484f817567e6
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992307"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="c1303-103">tipo de recurso resourceSpecificPermissionGrant</span><span class="sxs-lookup"><span data-stu-id="c1303-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="c1303-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1303-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1303-105">Um resourceSpecificPermissionGrant declara a permissão concedida a um aplicativo específico do AzureAD para uma instância de um recurso no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c1303-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="c1303-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c1303-106">Methods</span></span>

|  <span data-ttu-id="c1303-107">Método</span><span class="sxs-lookup"><span data-stu-id="c1303-107">Method</span></span>                                                                   |  <span data-ttu-id="c1303-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c1303-108">Return Type</span></span>                                                                     | <span data-ttu-id="c1303-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1303-109">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="c1303-110">Listar concessões de permissão de um chat</span><span class="sxs-lookup"><span data-stu-id="c1303-110">List permission grants of a chat</span></span>](../api/chat-list-permissiongrants.md)   | <span data-ttu-id="c1303-111">[coleção resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="c1303-111">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="c1303-112">Listar permissões concedidas em um chat específico.</span><span class="sxs-lookup"><span data-stu-id="c1303-112">List permissions that have been granted in a specific chat.</span></span>  |
|[<span data-ttu-id="c1303-113">Listar concessões de permissão de um grupo</span><span class="sxs-lookup"><span data-stu-id="c1303-113">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="c1303-114">[coleção resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="c1303-114">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="c1303-115">Listar permissões concedidas em um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="c1303-115">List permissions that have been granted in a specific group.</span></span> |
|[<span data-ttu-id="c1303-116">Listar concessões de permissão de uma equipe</span><span class="sxs-lookup"><span data-stu-id="c1303-116">List permission grants of a team</span></span>](../api/team-list-permissiongrants.md)   | <span data-ttu-id="c1303-117">[coleção resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="c1303-117">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="c1303-118">Listar permissões concedidas em uma equipe específica.</span><span class="sxs-lookup"><span data-stu-id="c1303-118">List permissions that have been granted in a specific team.</span></span>  |

## <a name="properties"></a><span data-ttu-id="c1303-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1303-119">Properties</span></span>

| <span data-ttu-id="c1303-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1303-120">Property</span></span>        | <span data-ttu-id="c1303-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1303-121">Type</span></span>          | <span data-ttu-id="c1303-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1303-122">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="c1303-123">id</span><span class="sxs-lookup"><span data-stu-id="c1303-123">id</span></span>              | <span data-ttu-id="c1303-124">string</span><span class="sxs-lookup"><span data-stu-id="c1303-124">string</span></span>        | <span data-ttu-id="c1303-125">O identificador exclusivo da concessão de permissão específica do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1303-125">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="c1303-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1303-126">Read-only.</span></span>           |
| <span data-ttu-id="c1303-127">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1303-127">deletedDateTime</span></span> | <span data-ttu-id="c1303-128">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1303-128">dateTimeOffset</span></span>| <span data-ttu-id="c1303-129">Não usado.</span><span class="sxs-lookup"><span data-stu-id="c1303-129">Not used.</span></span>                                                                             |
| <span data-ttu-id="c1303-130">clientId</span><span class="sxs-lookup"><span data-stu-id="c1303-130">clientId</span></span>        | <span data-ttu-id="c1303-131">string</span><span class="sxs-lookup"><span data-stu-id="c1303-131">string</span></span>        | <span data-ttu-id="c1303-132">ID do aplicativo do Azure AD que recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="c1303-132">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="c1303-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1303-133">Read-only.</span></span>                            |
| <span data-ttu-id="c1303-134">clientAppId</span><span class="sxs-lookup"><span data-stu-id="c1303-134">clientAppId</span></span>     | <span data-ttu-id="c1303-135">string</span><span class="sxs-lookup"><span data-stu-id="c1303-135">string</span></span>        | <span data-ttu-id="c1303-136">ID da entidade de serviço do aplicativo do Azure AD que recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="c1303-136">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="c1303-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1303-137">Read-only.</span></span>   |
| <span data-ttu-id="c1303-138">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="c1303-138">resourceAppId</span></span>   | <span data-ttu-id="c1303-139">string</span><span class="sxs-lookup"><span data-stu-id="c1303-139">string</span></span>        | <span data-ttu-id="c1303-140">ID do aplicativo do Azure AD que está hospedando o recurso.</span><span class="sxs-lookup"><span data-stu-id="c1303-140">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="c1303-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1303-141">Read-only.</span></span>                        |
| <span data-ttu-id="c1303-142">permissionType</span><span class="sxs-lookup"><span data-stu-id="c1303-142">permissionType</span></span>  | <span data-ttu-id="c1303-143">string</span><span class="sxs-lookup"><span data-stu-id="c1303-143">string</span></span>        | <span data-ttu-id="c1303-144">O tipo de permissão.</span><span class="sxs-lookup"><span data-stu-id="c1303-144">The type of permission.</span></span> <span data-ttu-id="c1303-145">Os valores possíveis são: `Application` e `Delegated`.</span><span class="sxs-lookup"><span data-stu-id="c1303-145">Possible values are: `Application`, `Delegated`.</span></span> <span data-ttu-id="c1303-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1303-146">Read-only.</span></span> |
| <span data-ttu-id="c1303-147">permission</span><span class="sxs-lookup"><span data-stu-id="c1303-147">permission</span></span>      | <span data-ttu-id="c1303-148">string</span><span class="sxs-lookup"><span data-stu-id="c1303-148">string</span></span>        | <span data-ttu-id="c1303-149">O nome da permissão.</span><span class="sxs-lookup"><span data-stu-id="c1303-149">The name of the permission.</span></span> <span data-ttu-id="c1303-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1303-150">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="c1303-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1303-151">JSON representation</span></span>

<span data-ttu-id="c1303-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1303-152">The following is a JSON representation of the resource.</span></span>

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


