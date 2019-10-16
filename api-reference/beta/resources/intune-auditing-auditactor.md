---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5fdb804dc293214fbcd7d937adb9ebdf959ea5fa
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538515"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="5849f-103">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="5849f-103">auditActor resource type</span></span>

> <span data-ttu-id="5849f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5849f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5849f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5849f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5849f-106">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="5849f-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="5849f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5849f-107">Properties</span></span>
|<span data-ttu-id="5849f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5849f-108">Property</span></span>|<span data-ttu-id="5849f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5849f-109">Type</span></span>|<span data-ttu-id="5849f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5849f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5849f-111">type</span><span class="sxs-lookup"><span data-stu-id="5849f-111">type</span></span>|<span data-ttu-id="5849f-112">String</span><span class="sxs-lookup"><span data-stu-id="5849f-112">String</span></span>|<span data-ttu-id="5849f-113">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="5849f-113">Actor Type.</span></span>|
|<span data-ttu-id="5849f-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="5849f-114">userPermissions</span></span>|<span data-ttu-id="5849f-115">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5849f-115">String collection</span></span>|<span data-ttu-id="5849f-116">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="5849f-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="5849f-117">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="5849f-117">applicationId</span></span>|<span data-ttu-id="5849f-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5849f-118">String</span></span>|<span data-ttu-id="5849f-119">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="5849f-119">AAD Application Id.</span></span>|
|<span data-ttu-id="5849f-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="5849f-120">applicationDisplayName</span></span>|<span data-ttu-id="5849f-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5849f-121">String</span></span>|<span data-ttu-id="5849f-122">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5849f-122">Name of the Application.</span></span>|
|<span data-ttu-id="5849f-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5849f-123">userPrincipalName</span></span>|<span data-ttu-id="5849f-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5849f-124">String</span></span>|<span data-ttu-id="5849f-125">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="5849f-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="5849f-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="5849f-126">servicePrincipalName</span></span>|<span data-ttu-id="5849f-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5849f-127">String</span></span>|<span data-ttu-id="5849f-128">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="5849f-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="5849f-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="5849f-129">ipAddress</span></span>|<span data-ttu-id="5849f-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5849f-130">String</span></span>|<span data-ttu-id="5849f-131">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="5849f-131">IPAddress.</span></span>|
|<span data-ttu-id="5849f-132">userId</span><span class="sxs-lookup"><span data-stu-id="5849f-132">userId</span></span>|<span data-ttu-id="5849f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5849f-133">String</span></span>|<span data-ttu-id="5849f-134">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="5849f-134">User Id.</span></span>|
|<span data-ttu-id="5849f-135">scopeTags</span><span class="sxs-lookup"><span data-stu-id="5849f-135">scopeTags</span></span>|<span data-ttu-id="5849f-136">coleção [scopeTagInfo](../resources/intune-auditing-scopetaginfo.md)</span><span class="sxs-lookup"><span data-stu-id="5849f-136">[scopeTagInfo](../resources/intune-auditing-scopetaginfo.md) collection</span></span>|<span data-ttu-id="5849f-137">Lista de marcas de escopo de usuário quando a auditoria foi realizada.</span><span class="sxs-lookup"><span data-stu-id="5849f-137">List of user scope tags when the audit was performed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5849f-138">Relações</span><span class="sxs-lookup"><span data-stu-id="5849f-138">Relationships</span></span>
<span data-ttu-id="5849f-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5849f-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5849f-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5849f-140">JSON Representation</span></span>
<span data-ttu-id="5849f-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5849f-141">Here is a JSON representation of the resource.</span></span>
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
  "scopeTags": [
    {
      "@odata.type": "microsoft.graph.scopeTagInfo",
      "scopeTagName": "String",
      "scopeTagId": "String"
    }
  ]
}
```



