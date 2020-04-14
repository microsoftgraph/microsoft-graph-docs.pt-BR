---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 173afc06c20e01406172cf2bc6b8c785aac55aa9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43403200"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="6fbba-103">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="6fbba-103">auditActor resource type</span></span>

<span data-ttu-id="6fbba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fbba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fbba-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6fbba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fbba-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6fbba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fbba-107">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="6fbba-107">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="6fbba-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6fbba-108">Properties</span></span>
|<span data-ttu-id="6fbba-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fbba-109">Property</span></span>|<span data-ttu-id="6fbba-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fbba-110">Type</span></span>|<span data-ttu-id="6fbba-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fbba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fbba-112">type</span><span class="sxs-lookup"><span data-stu-id="6fbba-112">type</span></span>|<span data-ttu-id="6fbba-113">String</span><span class="sxs-lookup"><span data-stu-id="6fbba-113">String</span></span>|<span data-ttu-id="6fbba-114">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="6fbba-114">Actor Type.</span></span>|
|<span data-ttu-id="6fbba-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="6fbba-115">userPermissions</span></span>|<span data-ttu-id="6fbba-116">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6fbba-116">String collection</span></span>|<span data-ttu-id="6fbba-117">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="6fbba-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="6fbba-118">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="6fbba-118">applicationId</span></span>|<span data-ttu-id="6fbba-119">String</span><span class="sxs-lookup"><span data-stu-id="6fbba-119">String</span></span>|<span data-ttu-id="6fbba-120">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="6fbba-120">AAD Application Id.</span></span>|
|<span data-ttu-id="6fbba-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="6fbba-121">applicationDisplayName</span></span>|<span data-ttu-id="6fbba-122">String</span><span class="sxs-lookup"><span data-stu-id="6fbba-122">String</span></span>|<span data-ttu-id="6fbba-123">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6fbba-123">Name of the Application.</span></span>|
|<span data-ttu-id="6fbba-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6fbba-124">userPrincipalName</span></span>|<span data-ttu-id="6fbba-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6fbba-125">String</span></span>|<span data-ttu-id="6fbba-126">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="6fbba-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="6fbba-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="6fbba-127">servicePrincipalName</span></span>|<span data-ttu-id="6fbba-128">String</span><span class="sxs-lookup"><span data-stu-id="6fbba-128">String</span></span>|<span data-ttu-id="6fbba-129">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="6fbba-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="6fbba-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="6fbba-130">ipAddress</span></span>|<span data-ttu-id="6fbba-131">String</span><span class="sxs-lookup"><span data-stu-id="6fbba-131">String</span></span>|<span data-ttu-id="6fbba-132">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="6fbba-132">IPAddress.</span></span>|
|<span data-ttu-id="6fbba-133">userId</span><span class="sxs-lookup"><span data-stu-id="6fbba-133">userId</span></span>|<span data-ttu-id="6fbba-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6fbba-134">String</span></span>|<span data-ttu-id="6fbba-135">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="6fbba-135">User Id.</span></span>|
|<span data-ttu-id="6fbba-136">userRoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="6fbba-136">userRoleScopeTags</span></span>|<span data-ttu-id="6fbba-137">coleção [roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md)</span><span class="sxs-lookup"><span data-stu-id="6fbba-137">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) collection</span></span>|<span data-ttu-id="6fbba-138">Lista de marcas de escopo de usuário quando a auditoria foi realizada.</span><span class="sxs-lookup"><span data-stu-id="6fbba-138">List of user scope tags when the audit was performed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fbba-139">Relações</span><span class="sxs-lookup"><span data-stu-id="6fbba-139">Relationships</span></span>
<span data-ttu-id="6fbba-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6fbba-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fbba-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6fbba-141">JSON Representation</span></span>
<span data-ttu-id="6fbba-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6fbba-142">Here is a JSON representation of the resource.</span></span>
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
  ]
}
```



