---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1d54d34081c931df442afa6d6d0e569de75fb652
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797434"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="75c08-103">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="75c08-103">auditActor resource type</span></span>

> <span data-ttu-id="75c08-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75c08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75c08-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75c08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75c08-106">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="75c08-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="75c08-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75c08-107">Properties</span></span>
|<span data-ttu-id="75c08-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75c08-108">Property</span></span>|<span data-ttu-id="75c08-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="75c08-109">Type</span></span>|<span data-ttu-id="75c08-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="75c08-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75c08-111">type</span><span class="sxs-lookup"><span data-stu-id="75c08-111">type</span></span>|<span data-ttu-id="75c08-112">String</span><span class="sxs-lookup"><span data-stu-id="75c08-112">String</span></span>|<span data-ttu-id="75c08-113">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="75c08-113">Actor Type.</span></span>|
|<span data-ttu-id="75c08-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="75c08-114">userPermissions</span></span>|<span data-ttu-id="75c08-115">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75c08-115">String collection</span></span>|<span data-ttu-id="75c08-116">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="75c08-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="75c08-117">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="75c08-117">applicationId</span></span>|<span data-ttu-id="75c08-118">String</span><span class="sxs-lookup"><span data-stu-id="75c08-118">String</span></span>|<span data-ttu-id="75c08-119">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="75c08-119">AAD Application Id.</span></span>|
|<span data-ttu-id="75c08-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="75c08-120">applicationDisplayName</span></span>|<span data-ttu-id="75c08-121">String</span><span class="sxs-lookup"><span data-stu-id="75c08-121">String</span></span>|<span data-ttu-id="75c08-122">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75c08-122">Name of the Application.</span></span>|
|<span data-ttu-id="75c08-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="75c08-123">userPrincipalName</span></span>|<span data-ttu-id="75c08-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75c08-124">String</span></span>|<span data-ttu-id="75c08-125">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="75c08-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="75c08-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="75c08-126">servicePrincipalName</span></span>|<span data-ttu-id="75c08-127">String</span><span class="sxs-lookup"><span data-stu-id="75c08-127">String</span></span>|<span data-ttu-id="75c08-128">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="75c08-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="75c08-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="75c08-129">ipAddress</span></span>|<span data-ttu-id="75c08-130">String</span><span class="sxs-lookup"><span data-stu-id="75c08-130">String</span></span>|<span data-ttu-id="75c08-131">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="75c08-131">IPAddress.</span></span>|
|<span data-ttu-id="75c08-132">userId</span><span class="sxs-lookup"><span data-stu-id="75c08-132">userId</span></span>|<span data-ttu-id="75c08-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75c08-133">String</span></span>|<span data-ttu-id="75c08-134">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="75c08-134">User Id.</span></span>|
|<span data-ttu-id="75c08-135">userRoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="75c08-135">userRoleScopeTags</span></span>|<span data-ttu-id="75c08-136">coleção [roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md)</span><span class="sxs-lookup"><span data-stu-id="75c08-136">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) collection</span></span>|<span data-ttu-id="75c08-137">Lista de marcas de escopo de usuário quando a auditoria foi realizada.</span><span class="sxs-lookup"><span data-stu-id="75c08-137">List of user scope tags when the audit was performed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75c08-138">Relações</span><span class="sxs-lookup"><span data-stu-id="75c08-138">Relationships</span></span>
<span data-ttu-id="75c08-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="75c08-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75c08-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75c08-140">JSON Representation</span></span>
<span data-ttu-id="75c08-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75c08-141">Here is a JSON representation of the resource.</span></span>
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



