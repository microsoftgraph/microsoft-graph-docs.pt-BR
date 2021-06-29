---
title: tipo de recurso resourceSpecificPermissionGrant
description: Especifica a permissão que um aplicativo específico do Azure AD tem.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2fd6e9e09a092719f20de2c34f2120537cd00606
ms.sourcegitcommit: b5fbb1a715e3479bdd095ef00deb0c932eafc328
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2021
ms.locfileid: "53162193"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="37aad-103">tipo de recurso resourceSpecificPermissionGrant</span><span class="sxs-lookup"><span data-stu-id="37aad-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="37aad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37aad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37aad-105">Um resourceSpecificPermissionGrant declara a permissão concedida a um aplicativo específico do AzureAD para uma instância de um recurso no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="37aad-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

<span data-ttu-id="37aad-106">Para obter mais informações sobre a concessão de consentimento de aplicativos para acessar uma instância específica de um recurso, consulte [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span><span class="sxs-lookup"><span data-stu-id="37aad-106">For more information about granting apps consent to access a specific instance of a resource, see [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

## <a name="methods"></a><span data-ttu-id="37aad-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="37aad-107">Methods</span></span>

|  <span data-ttu-id="37aad-108">Método</span><span class="sxs-lookup"><span data-stu-id="37aad-108">Method</span></span>                                                                   |  <span data-ttu-id="37aad-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="37aad-109">Return Type</span></span>                                                                     | <span data-ttu-id="37aad-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="37aad-110">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="37aad-111">Listar as concessões de permissões de um grupo</span><span class="sxs-lookup"><span data-stu-id="37aad-111">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="37aad-112">Coleção [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="37aad-112">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="37aad-113">Listar permissões específicas de recursos que foram concedidas em um grupo [específico.](group.md)</span><span class="sxs-lookup"><span data-stu-id="37aad-113">List resource-specific permissions that have been granted in a specific [group](group.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="37aad-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37aad-114">Properties</span></span>

| <span data-ttu-id="37aad-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37aad-115">Property</span></span>        | <span data-ttu-id="37aad-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="37aad-116">Type</span></span>          | <span data-ttu-id="37aad-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="37aad-117">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="37aad-118">id</span><span class="sxs-lookup"><span data-stu-id="37aad-118">id</span></span>              | <span data-ttu-id="37aad-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37aad-119">string</span></span>        | <span data-ttu-id="37aad-120">O identificador exclusivo da concessão de permissão específica do recurso.</span><span class="sxs-lookup"><span data-stu-id="37aad-120">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="37aad-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37aad-121">Read-only.</span></span>           |
| <span data-ttu-id="37aad-122">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="37aad-122">deletedDateTime</span></span> | <span data-ttu-id="37aad-123">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37aad-123">dateTimeOffset</span></span>| <span data-ttu-id="37aad-124">Não usado.</span><span class="sxs-lookup"><span data-stu-id="37aad-124">Not used.</span></span>                                                                             |
| <span data-ttu-id="37aad-125">clientId</span><span class="sxs-lookup"><span data-stu-id="37aad-125">clientId</span></span>        | <span data-ttu-id="37aad-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37aad-126">string</span></span>        | <span data-ttu-id="37aad-127">ID do aplicativo do Azure AD que recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="37aad-127">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="37aad-128">Só leitura.</span><span class="sxs-lookup"><span data-stu-id="37aad-128">Read-only.</span></span>                            |
| <span data-ttu-id="37aad-129">clientAppId</span><span class="sxs-lookup"><span data-stu-id="37aad-129">clientAppId</span></span>     | <span data-ttu-id="37aad-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37aad-130">string</span></span>        | <span data-ttu-id="37aad-131">ID da entidade de serviço do aplicativo do Azure AD que recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="37aad-131">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="37aad-132">Só leitura.</span><span class="sxs-lookup"><span data-stu-id="37aad-132">Read-only.</span></span>   |
| <span data-ttu-id="37aad-133">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="37aad-133">resourceAppId</span></span>   | <span data-ttu-id="37aad-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37aad-134">string</span></span>        | <span data-ttu-id="37aad-135">ID do aplicativo do Azure AD que está hospedando o recurso.</span><span class="sxs-lookup"><span data-stu-id="37aad-135">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="37aad-136">Só leitura.</span><span class="sxs-lookup"><span data-stu-id="37aad-136">Read-only.</span></span>                        |
| <span data-ttu-id="37aad-137">permissionType</span><span class="sxs-lookup"><span data-stu-id="37aad-137">permissionType</span></span>  | <span data-ttu-id="37aad-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37aad-138">string</span></span>        | <span data-ttu-id="37aad-139">O tipo de permissão.</span><span class="sxs-lookup"><span data-stu-id="37aad-139">The type of permission.</span></span> <span data-ttu-id="37aad-140">Os valores possíveis são: `Application` e `Delegated`.</span><span class="sxs-lookup"><span data-stu-id="37aad-140">Possible values are: `Application`, `Delegated`.</span></span> <span data-ttu-id="37aad-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37aad-141">Read-only.</span></span> |
| <span data-ttu-id="37aad-142">permission</span><span class="sxs-lookup"><span data-stu-id="37aad-142">permission</span></span>      | <span data-ttu-id="37aad-143">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37aad-143">string</span></span>        | <span data-ttu-id="37aad-144">O nome da permissão específica do recurso.</span><span class="sxs-lookup"><span data-stu-id="37aad-144">The name of the resource-specific permission.</span></span> <span data-ttu-id="37aad-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37aad-145">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="37aad-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37aad-146">JSON representation</span></span>

<span data-ttu-id="37aad-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37aad-147">The following is a JSON representation of the resource.</span></span>

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