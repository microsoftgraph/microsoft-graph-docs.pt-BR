---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01dd1df7e273e9ef2bbd6fabb9a0ea0203e5347f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295534"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="3dc2b-103">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="3dc2b-103">auditActor resource type</span></span>

<span data-ttu-id="3dc2b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3dc2b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3dc2b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3dc2b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3dc2b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3dc2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3dc2b-107">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="3dc2b-107">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="3dc2b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3dc2b-108">Properties</span></span>
|<span data-ttu-id="3dc2b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3dc2b-109">Property</span></span>|<span data-ttu-id="3dc2b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3dc2b-110">Type</span></span>|<span data-ttu-id="3dc2b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3dc2b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dc2b-112">tipo</span><span class="sxs-lookup"><span data-stu-id="3dc2b-112">type</span></span>|<span data-ttu-id="3dc2b-113">String</span><span class="sxs-lookup"><span data-stu-id="3dc2b-113">String</span></span>|<span data-ttu-id="3dc2b-114">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="3dc2b-114">Actor Type.</span></span>|
|<span data-ttu-id="3dc2b-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="3dc2b-115">userPermissions</span></span>|<span data-ttu-id="3dc2b-116">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3dc2b-116">String collection</span></span>|<span data-ttu-id="3dc2b-117">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="3dc2b-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="3dc2b-118">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="3dc2b-118">applicationId</span></span>|<span data-ttu-id="3dc2b-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3dc2b-119">String</span></span>|<span data-ttu-id="3dc2b-120">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="3dc2b-120">AAD Application Id.</span></span>|
|<span data-ttu-id="3dc2b-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="3dc2b-121">applicationDisplayName</span></span>|<span data-ttu-id="3dc2b-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3dc2b-122">String</span></span>|<span data-ttu-id="3dc2b-123">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3dc2b-123">Name of the Application.</span></span>|
|<span data-ttu-id="3dc2b-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3dc2b-124">userPrincipalName</span></span>|<span data-ttu-id="3dc2b-125">String</span><span class="sxs-lookup"><span data-stu-id="3dc2b-125">String</span></span>|<span data-ttu-id="3dc2b-126">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="3dc2b-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="3dc2b-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="3dc2b-127">servicePrincipalName</span></span>|<span data-ttu-id="3dc2b-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3dc2b-128">String</span></span>|<span data-ttu-id="3dc2b-129">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="3dc2b-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="3dc2b-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="3dc2b-130">ipAddress</span></span>|<span data-ttu-id="3dc2b-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3dc2b-131">String</span></span>|<span data-ttu-id="3dc2b-132">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="3dc2b-132">IPAddress.</span></span>|
|<span data-ttu-id="3dc2b-133">userId</span><span class="sxs-lookup"><span data-stu-id="3dc2b-133">userId</span></span>|<span data-ttu-id="3dc2b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3dc2b-134">String</span></span>|<span data-ttu-id="3dc2b-135">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="3dc2b-135">User Id.</span></span>|
|<span data-ttu-id="3dc2b-136">userRoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="3dc2b-136">userRoleScopeTags</span></span>|<span data-ttu-id="3dc2b-137">coleção [roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md)</span><span class="sxs-lookup"><span data-stu-id="3dc2b-137">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) collection</span></span>|<span data-ttu-id="3dc2b-138">Lista de marcas de escopo de usuário quando a auditoria foi realizada.</span><span class="sxs-lookup"><span data-stu-id="3dc2b-138">List of user scope tags when the audit was performed.</span></span>|
|<span data-ttu-id="3dc2b-139">remoteTenantId</span><span class="sxs-lookup"><span data-stu-id="3dc2b-139">remoteTenantId</span></span>|<span data-ttu-id="3dc2b-140">String</span><span class="sxs-lookup"><span data-stu-id="3dc2b-140">String</span></span>|<span data-ttu-id="3dc2b-141">ID de locatário remoto</span><span class="sxs-lookup"><span data-stu-id="3dc2b-141">Remote Tenant Id</span></span>|
|<span data-ttu-id="3dc2b-142">remoteUserId</span><span class="sxs-lookup"><span data-stu-id="3dc2b-142">remoteUserId</span></span>|<span data-ttu-id="3dc2b-143">String</span><span class="sxs-lookup"><span data-stu-id="3dc2b-143">String</span></span>|<span data-ttu-id="3dc2b-144">ID de usuário remoto</span><span class="sxs-lookup"><span data-stu-id="3dc2b-144">Remote User Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="3dc2b-145">Relações</span><span class="sxs-lookup"><span data-stu-id="3dc2b-145">Relationships</span></span>
<span data-ttu-id="3dc2b-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3dc2b-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3dc2b-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3dc2b-147">JSON Representation</span></span>
<span data-ttu-id="3dc2b-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3dc2b-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String",
  "userRoleScopeTags": [
    {
      "@odata.type": "microsoft.graph.roleScopeTagInfo",
      "displayName": "String",
      "roleScopeTagId": "String"
    }
  ],
  "remoteTenantId": "String",
  "remoteUserId": "String"
}
```




