---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd8edf9b9ab9b0513e77bbef6ce04dfcd5d4a1a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019562"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="d571e-103">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="d571e-103">auditActor resource type</span></span>

<span data-ttu-id="d571e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d571e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d571e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d571e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d571e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d571e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d571e-107">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="d571e-107">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="d571e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d571e-108">Properties</span></span>
|<span data-ttu-id="d571e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d571e-109">Property</span></span>|<span data-ttu-id="d571e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d571e-110">Type</span></span>|<span data-ttu-id="d571e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d571e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d571e-112">tipo</span><span class="sxs-lookup"><span data-stu-id="d571e-112">type</span></span>|<span data-ttu-id="d571e-113">String</span><span class="sxs-lookup"><span data-stu-id="d571e-113">String</span></span>|<span data-ttu-id="d571e-114">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="d571e-114">Actor Type.</span></span>|
|<span data-ttu-id="d571e-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="d571e-115">userPermissions</span></span>|<span data-ttu-id="d571e-116">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d571e-116">String collection</span></span>|<span data-ttu-id="d571e-117">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="d571e-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="d571e-118">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="d571e-118">applicationId</span></span>|<span data-ttu-id="d571e-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d571e-119">String</span></span>|<span data-ttu-id="d571e-120">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="d571e-120">AAD Application Id.</span></span>|
|<span data-ttu-id="d571e-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="d571e-121">applicationDisplayName</span></span>|<span data-ttu-id="d571e-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d571e-122">String</span></span>|<span data-ttu-id="d571e-123">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d571e-123">Name of the Application.</span></span>|
|<span data-ttu-id="d571e-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d571e-124">userPrincipalName</span></span>|<span data-ttu-id="d571e-125">String</span><span class="sxs-lookup"><span data-stu-id="d571e-125">String</span></span>|<span data-ttu-id="d571e-126">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="d571e-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="d571e-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="d571e-127">servicePrincipalName</span></span>|<span data-ttu-id="d571e-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d571e-128">String</span></span>|<span data-ttu-id="d571e-129">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="d571e-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="d571e-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="d571e-130">ipAddress</span></span>|<span data-ttu-id="d571e-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d571e-131">String</span></span>|<span data-ttu-id="d571e-132">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="d571e-132">IPAddress.</span></span>|
|<span data-ttu-id="d571e-133">userId</span><span class="sxs-lookup"><span data-stu-id="d571e-133">userId</span></span>|<span data-ttu-id="d571e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d571e-134">String</span></span>|<span data-ttu-id="d571e-135">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="d571e-135">User Id.</span></span>|
|<span data-ttu-id="d571e-136">userRoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="d571e-136">userRoleScopeTags</span></span>|<span data-ttu-id="d571e-137">coleção [roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md)</span><span class="sxs-lookup"><span data-stu-id="d571e-137">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) collection</span></span>|<span data-ttu-id="d571e-138">Lista de marcas de escopo de usuário quando a auditoria foi realizada.</span><span class="sxs-lookup"><span data-stu-id="d571e-138">List of user scope tags when the audit was performed.</span></span>|
|<span data-ttu-id="d571e-139">remoteTenantId</span><span class="sxs-lookup"><span data-stu-id="d571e-139">remoteTenantId</span></span>|<span data-ttu-id="d571e-140">String</span><span class="sxs-lookup"><span data-stu-id="d571e-140">String</span></span>|<span data-ttu-id="d571e-141">ID de locatário remoto</span><span class="sxs-lookup"><span data-stu-id="d571e-141">Remote Tenant Id</span></span>|
|<span data-ttu-id="d571e-142">remoteUserId</span><span class="sxs-lookup"><span data-stu-id="d571e-142">remoteUserId</span></span>|<span data-ttu-id="d571e-143">String</span><span class="sxs-lookup"><span data-stu-id="d571e-143">String</span></span>|<span data-ttu-id="d571e-144">ID de usuário remoto</span><span class="sxs-lookup"><span data-stu-id="d571e-144">Remote User Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="d571e-145">Relações</span><span class="sxs-lookup"><span data-stu-id="d571e-145">Relationships</span></span>
<span data-ttu-id="d571e-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d571e-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d571e-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d571e-147">JSON Representation</span></span>
<span data-ttu-id="d571e-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d571e-148">Here is a JSON representation of the resource.</span></span>
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






