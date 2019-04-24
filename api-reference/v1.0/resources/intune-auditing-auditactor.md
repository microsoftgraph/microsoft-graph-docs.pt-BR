---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 632e3018f606b62171461b4b1235ccdafc6b1b5a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584702"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="6a4b1-103">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="6a4b1-103">auditActor resource type</span></span>

> <span data-ttu-id="6a4b1-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a4b1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a4b1-105">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="6a4b1-105">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="6a4b1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a4b1-106">Properties</span></span>
|<span data-ttu-id="6a4b1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a4b1-107">Property</span></span>|<span data-ttu-id="6a4b1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a4b1-108">Type</span></span>|<span data-ttu-id="6a4b1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a4b1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a4b1-110">type</span><span class="sxs-lookup"><span data-stu-id="6a4b1-110">type</span></span>|<span data-ttu-id="6a4b1-111">String</span><span class="sxs-lookup"><span data-stu-id="6a4b1-111">String</span></span>|<span data-ttu-id="6a4b1-112">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="6a4b1-112">Actor Type.</span></span>|
|<span data-ttu-id="6a4b1-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="6a4b1-113">userPermissions</span></span>|<span data-ttu-id="6a4b1-114">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a4b1-114">String collection</span></span>|<span data-ttu-id="6a4b1-115">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="6a4b1-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="6a4b1-116">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="6a4b1-116">applicationId</span></span>|<span data-ttu-id="6a4b1-117">String</span><span class="sxs-lookup"><span data-stu-id="6a4b1-117">String</span></span>|<span data-ttu-id="6a4b1-118">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="6a4b1-118">AAD Application Id.</span></span>|
|<span data-ttu-id="6a4b1-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="6a4b1-119">applicationDisplayName</span></span>|<span data-ttu-id="6a4b1-120">String</span><span class="sxs-lookup"><span data-stu-id="6a4b1-120">String</span></span>|<span data-ttu-id="6a4b1-121">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6a4b1-121">Name of the Application.</span></span>|
|<span data-ttu-id="6a4b1-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6a4b1-122">userPrincipalName</span></span>|<span data-ttu-id="6a4b1-123">String</span><span class="sxs-lookup"><span data-stu-id="6a4b1-123">String</span></span>|<span data-ttu-id="6a4b1-124">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="6a4b1-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="6a4b1-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="6a4b1-125">servicePrincipalName</span></span>|<span data-ttu-id="6a4b1-126">String</span><span class="sxs-lookup"><span data-stu-id="6a4b1-126">String</span></span>|<span data-ttu-id="6a4b1-127">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="6a4b1-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="6a4b1-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="6a4b1-128">ipAddress</span></span>|<span data-ttu-id="6a4b1-129">String</span><span class="sxs-lookup"><span data-stu-id="6a4b1-129">String</span></span>|<span data-ttu-id="6a4b1-130">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="6a4b1-130">IPAddress.</span></span>|
|<span data-ttu-id="6a4b1-131">userId</span><span class="sxs-lookup"><span data-stu-id="6a4b1-131">userId</span></span>|<span data-ttu-id="6a4b1-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a4b1-132">String</span></span>|<span data-ttu-id="6a4b1-133">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="6a4b1-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a4b1-134">Relações</span><span class="sxs-lookup"><span data-stu-id="6a4b1-134">Relationships</span></span>
<span data-ttu-id="6a4b1-135">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6a4b1-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a4b1-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a4b1-136">JSON Representation</span></span>
<span data-ttu-id="6a4b1-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a4b1-137">Here is a JSON representation of the resource.</span></span>
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



