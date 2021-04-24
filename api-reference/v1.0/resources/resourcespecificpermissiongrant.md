---
title: tipo de recurso resourceSpecificPermissionGrant
description: Especifica a permissão que um aplicativo específico do Azure AD tem.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 769c4d405473ef800b92fbecb8797588cf59eb57
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944287"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="8dc59-103">tipo de recurso resourceSpecificPermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8dc59-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="8dc59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dc59-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8dc59-105">Um resourceSpecificPermissionGrant declara a permissão concedida a um aplicativo específico do AzureAD para uma instância de um recurso no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8dc59-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="8dc59-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8dc59-106">Methods</span></span>

|  <span data-ttu-id="8dc59-107">Método</span><span class="sxs-lookup"><span data-stu-id="8dc59-107">Method</span></span>                                                                   |  <span data-ttu-id="8dc59-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8dc59-108">Return Type</span></span>                                                                     | <span data-ttu-id="8dc59-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dc59-109">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="8dc59-110">Listar concessões de permissão de um grupo</span><span class="sxs-lookup"><span data-stu-id="8dc59-110">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="8dc59-111">[coleção resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="8dc59-111">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="8dc59-112">Listar permissões concedidas em um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="8dc59-112">List permissions that have been granted in a specific group.</span></span> |

## <a name="properties"></a><span data-ttu-id="8dc59-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8dc59-113">Properties</span></span>

| <span data-ttu-id="8dc59-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8dc59-114">Property</span></span>        | <span data-ttu-id="8dc59-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dc59-115">Type</span></span>          | <span data-ttu-id="8dc59-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dc59-116">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="8dc59-117">id</span><span class="sxs-lookup"><span data-stu-id="8dc59-117">id</span></span>              | <span data-ttu-id="8dc59-118">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc59-118">string</span></span>        | <span data-ttu-id="8dc59-119">O identificador exclusivo da concessão de permissão específica do recurso.</span><span class="sxs-lookup"><span data-stu-id="8dc59-119">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="8dc59-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8dc59-120">Read-only.</span></span>           |
| <span data-ttu-id="8dc59-121">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="8dc59-121">deletedDateTime</span></span> | <span data-ttu-id="8dc59-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dc59-122">dateTimeOffset</span></span>| <span data-ttu-id="8dc59-123">Não usado.</span><span class="sxs-lookup"><span data-stu-id="8dc59-123">Not used.</span></span>                                                                             |
| <span data-ttu-id="8dc59-124">clientId</span><span class="sxs-lookup"><span data-stu-id="8dc59-124">clientId</span></span>        | <span data-ttu-id="8dc59-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc59-125">string</span></span>        | <span data-ttu-id="8dc59-126">ID do aplicativo do Azure AD que recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="8dc59-126">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="8dc59-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8dc59-127">Read-only.</span></span>                            |
| <span data-ttu-id="8dc59-128">clientAppId</span><span class="sxs-lookup"><span data-stu-id="8dc59-128">clientAppId</span></span>     | <span data-ttu-id="8dc59-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc59-129">string</span></span>        | <span data-ttu-id="8dc59-130">ID da entidade de serviço do aplicativo do Azure AD que recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="8dc59-130">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="8dc59-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8dc59-131">Read-only.</span></span>   |
| <span data-ttu-id="8dc59-132">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="8dc59-132">resourceAppId</span></span>   | <span data-ttu-id="8dc59-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc59-133">string</span></span>        | <span data-ttu-id="8dc59-134">ID do aplicativo do Azure AD que está hospedando o recurso.</span><span class="sxs-lookup"><span data-stu-id="8dc59-134">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="8dc59-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8dc59-135">Read-only.</span></span>                        |
| <span data-ttu-id="8dc59-136">permissionType</span><span class="sxs-lookup"><span data-stu-id="8dc59-136">permissionType</span></span>  | <span data-ttu-id="8dc59-137">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc59-137">string</span></span>        | <span data-ttu-id="8dc59-138">O tipo de permissão.</span><span class="sxs-lookup"><span data-stu-id="8dc59-138">The type of permission.</span></span> <span data-ttu-id="8dc59-139">Os valores possíveis são: `Application` e `Delegated`.</span><span class="sxs-lookup"><span data-stu-id="8dc59-139">Possible values are: `Application`, `Delegated`.</span></span> <span data-ttu-id="8dc59-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8dc59-140">Read-only.</span></span> |
| <span data-ttu-id="8dc59-141">permission</span><span class="sxs-lookup"><span data-stu-id="8dc59-141">permission</span></span>      | <span data-ttu-id="8dc59-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc59-142">string</span></span>        | <span data-ttu-id="8dc59-143">O nome da permissão.</span><span class="sxs-lookup"><span data-stu-id="8dc59-143">The name of the permission.</span></span> <span data-ttu-id="8dc59-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8dc59-144">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="8dc59-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8dc59-145">JSON representation</span></span>

<span data-ttu-id="8dc59-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8dc59-146">The following is a JSON representation of the resource.</span></span>

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