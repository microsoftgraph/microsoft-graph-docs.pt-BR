---
title: tipo de recurso resourceSpecificPermissionGrant
description: Especifica a permissão que um aplicativo específico do Azure AD tem.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f100d5658b2ecdc07daf928594180b0ce6129594
ms.sourcegitcommit: b5fbb1a715e3479bdd095ef00deb0c932eafc328
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2021
ms.locfileid: "53162216"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="38e1a-103">tipo de recurso resourceSpecificPermissionGrant</span><span class="sxs-lookup"><span data-stu-id="38e1a-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="38e1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38e1a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38e1a-105">Um resourceSpecificPermissionGrant declara a permissão concedida a um aplicativo específico do AzureAD para uma instância de um recurso no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="38e1a-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

<span data-ttu-id="38e1a-106">Para obter mais informações sobre a concessão de consentimento de aplicativos para acessar uma instância específica de um recurso, consulte [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span><span class="sxs-lookup"><span data-stu-id="38e1a-106">For more information about granting apps consent to access a specific instance of a resource, see [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

## <a name="methods"></a><span data-ttu-id="38e1a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="38e1a-107">Methods</span></span>

|  <span data-ttu-id="38e1a-108">Método</span><span class="sxs-lookup"><span data-stu-id="38e1a-108">Method</span></span>                                                                   |  <span data-ttu-id="38e1a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="38e1a-109">Return Type</span></span>                                                                     | <span data-ttu-id="38e1a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="38e1a-110">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="38e1a-111">Listar concessões de permissão de um chat</span><span class="sxs-lookup"><span data-stu-id="38e1a-111">List permission grants of a chat</span></span>](../api/chat-list-permissiongrants.md)   | <span data-ttu-id="38e1a-112">Coleção [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="38e1a-112">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="38e1a-113">Listar permissões específicas de recursos que foram concedidas em um chat [específico.](chat.md)</span><span class="sxs-lookup"><span data-stu-id="38e1a-113">List resource-specific permissions that have been granted in a specific [chat](chat.md).</span></span>  |
|[<span data-ttu-id="38e1a-114">Listar as concessões de permissões de um grupo</span><span class="sxs-lookup"><span data-stu-id="38e1a-114">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="38e1a-115">Coleção [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="38e1a-115">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="38e1a-116">Listar permissões específicas de recursos que foram concedidas em um grupo [específico.](group.md)</span><span class="sxs-lookup"><span data-stu-id="38e1a-116">List resource-specific permissions that have been granted in a specific [group](group.md).</span></span> |
|[<span data-ttu-id="38e1a-117">Listar as concessões de permissões de uma equipe</span><span class="sxs-lookup"><span data-stu-id="38e1a-117">List permission grants of a team</span></span>](../api/team-list-permissiongrants.md) | <span data-ttu-id="38e1a-118">Coleção [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="38e1a-118">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="38e1a-119">Listar permissões específicas de recursos que foram concedidas em uma equipe [específica.](team.md)</span><span class="sxs-lookup"><span data-stu-id="38e1a-119">List resource-specific permissions that have been granted in a specific [team](team.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="38e1a-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38e1a-120">Properties</span></span>

| <span data-ttu-id="38e1a-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38e1a-121">Property</span></span>        | <span data-ttu-id="38e1a-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="38e1a-122">Type</span></span>          | <span data-ttu-id="38e1a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="38e1a-123">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="38e1a-124">id</span><span class="sxs-lookup"><span data-stu-id="38e1a-124">id</span></span>              | <span data-ttu-id="38e1a-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38e1a-125">string</span></span>        | <span data-ttu-id="38e1a-126">O identificador exclusivo da concessão de permissão específica do recurso.</span><span class="sxs-lookup"><span data-stu-id="38e1a-126">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="38e1a-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38e1a-127">Read-only.</span></span>           |
| <span data-ttu-id="38e1a-128">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="38e1a-128">deletedDateTime</span></span> | <span data-ttu-id="38e1a-129">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38e1a-129">dateTimeOffset</span></span>| <span data-ttu-id="38e1a-130">Não usado.</span><span class="sxs-lookup"><span data-stu-id="38e1a-130">Not used.</span></span>                                                                             |
| <span data-ttu-id="38e1a-131">clientId</span><span class="sxs-lookup"><span data-stu-id="38e1a-131">clientId</span></span>        | <span data-ttu-id="38e1a-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38e1a-132">string</span></span>        | <span data-ttu-id="38e1a-133">ID do aplicativo do Azure AD que recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="38e1a-133">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="38e1a-134">Só leitura.</span><span class="sxs-lookup"><span data-stu-id="38e1a-134">Read-only.</span></span>                            |
| <span data-ttu-id="38e1a-135">clientAppId</span><span class="sxs-lookup"><span data-stu-id="38e1a-135">clientAppId</span></span>     | <span data-ttu-id="38e1a-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38e1a-136">string</span></span>        | <span data-ttu-id="38e1a-137">ID da entidade de serviço do aplicativo do Azure AD que recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="38e1a-137">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="38e1a-138">Só leitura.</span><span class="sxs-lookup"><span data-stu-id="38e1a-138">Read-only.</span></span>   |
| <span data-ttu-id="38e1a-139">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="38e1a-139">resourceAppId</span></span>   | <span data-ttu-id="38e1a-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38e1a-140">string</span></span>        | <span data-ttu-id="38e1a-141">ID do aplicativo do Azure AD que está hospedando o recurso.</span><span class="sxs-lookup"><span data-stu-id="38e1a-141">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="38e1a-142">Só leitura.</span><span class="sxs-lookup"><span data-stu-id="38e1a-142">Read-only.</span></span>                        |
| <span data-ttu-id="38e1a-143">permissionType</span><span class="sxs-lookup"><span data-stu-id="38e1a-143">permissionType</span></span>  | <span data-ttu-id="38e1a-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38e1a-144">string</span></span>        | <span data-ttu-id="38e1a-145">O tipo de permissão.</span><span class="sxs-lookup"><span data-stu-id="38e1a-145">The type of permission.</span></span> <span data-ttu-id="38e1a-146">Os valores possíveis são: `Application` e `Delegated`.</span><span class="sxs-lookup"><span data-stu-id="38e1a-146">Possible values are: `Application`, `Delegated`.</span></span> <span data-ttu-id="38e1a-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38e1a-147">Read-only.</span></span> |
| <span data-ttu-id="38e1a-148">permission</span><span class="sxs-lookup"><span data-stu-id="38e1a-148">permission</span></span>      | <span data-ttu-id="38e1a-149">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38e1a-149">string</span></span>        | <span data-ttu-id="38e1a-150">O nome da permissão específica do recurso.</span><span class="sxs-lookup"><span data-stu-id="38e1a-150">The name of the resource-specific permission.</span></span> <span data-ttu-id="38e1a-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38e1a-151">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="38e1a-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38e1a-152">JSON representation</span></span>

<span data-ttu-id="38e1a-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38e1a-153">The following is a JSON representation of the resource.</span></span>

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


