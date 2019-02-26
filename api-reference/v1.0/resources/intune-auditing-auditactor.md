---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 632e3018f606b62171461b4b1235ccdafc6b1b5a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254454"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="1fa80-103">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="1fa80-103">auditActor resource type</span></span>

> <span data-ttu-id="1fa80-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1fa80-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fa80-105">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="1fa80-105">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="1fa80-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1fa80-106">Properties</span></span>
|<span data-ttu-id="1fa80-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fa80-107">Property</span></span>|<span data-ttu-id="1fa80-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fa80-108">Type</span></span>|<span data-ttu-id="1fa80-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fa80-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fa80-110">type</span><span class="sxs-lookup"><span data-stu-id="1fa80-110">type</span></span>|<span data-ttu-id="1fa80-111">String</span><span class="sxs-lookup"><span data-stu-id="1fa80-111">String</span></span>|<span data-ttu-id="1fa80-112">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="1fa80-112">Actor Type.</span></span>|
|<span data-ttu-id="1fa80-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="1fa80-113">userPermissions</span></span>|<span data-ttu-id="1fa80-114">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1fa80-114">String collection</span></span>|<span data-ttu-id="1fa80-115">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="1fa80-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="1fa80-116">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="1fa80-116">applicationId</span></span>|<span data-ttu-id="1fa80-117">String</span><span class="sxs-lookup"><span data-stu-id="1fa80-117">String</span></span>|<span data-ttu-id="1fa80-118">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="1fa80-118">AAD Application Id.</span></span>|
|<span data-ttu-id="1fa80-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="1fa80-119">applicationDisplayName</span></span>|<span data-ttu-id="1fa80-120">String</span><span class="sxs-lookup"><span data-stu-id="1fa80-120">String</span></span>|<span data-ttu-id="1fa80-121">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1fa80-121">Name of the Application.</span></span>|
|<span data-ttu-id="1fa80-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1fa80-122">userPrincipalName</span></span>|<span data-ttu-id="1fa80-123">String</span><span class="sxs-lookup"><span data-stu-id="1fa80-123">String</span></span>|<span data-ttu-id="1fa80-124">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="1fa80-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="1fa80-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="1fa80-125">servicePrincipalName</span></span>|<span data-ttu-id="1fa80-126">String</span><span class="sxs-lookup"><span data-stu-id="1fa80-126">String</span></span>|<span data-ttu-id="1fa80-127">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="1fa80-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="1fa80-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="1fa80-128">ipAddress</span></span>|<span data-ttu-id="1fa80-129">String</span><span class="sxs-lookup"><span data-stu-id="1fa80-129">String</span></span>|<span data-ttu-id="1fa80-130">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="1fa80-130">IPAddress.</span></span>|
|<span data-ttu-id="1fa80-131">userId</span><span class="sxs-lookup"><span data-stu-id="1fa80-131">userId</span></span>|<span data-ttu-id="1fa80-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1fa80-132">String</span></span>|<span data-ttu-id="1fa80-133">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="1fa80-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fa80-134">Relações</span><span class="sxs-lookup"><span data-stu-id="1fa80-134">Relationships</span></span>
<span data-ttu-id="1fa80-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1fa80-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1fa80-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1fa80-136">JSON Representation</span></span>
<span data-ttu-id="1fa80-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1fa80-137">Here is a JSON representation of the resource.</span></span>
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
  "userId": "String"
}
```



