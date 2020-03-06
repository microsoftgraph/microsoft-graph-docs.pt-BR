---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c10ac0a18f5bfcf68be56edc402c83d9882a8ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532738"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="2d8b7-103">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="2d8b7-103">auditActor resource type</span></span>

<span data-ttu-id="2d8b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d8b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d8b7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d8b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d8b7-106">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="2d8b7-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="2d8b7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d8b7-107">Properties</span></span>
|<span data-ttu-id="2d8b7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d8b7-108">Property</span></span>|<span data-ttu-id="2d8b7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d8b7-109">Type</span></span>|<span data-ttu-id="2d8b7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d8b7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d8b7-111">type</span><span class="sxs-lookup"><span data-stu-id="2d8b7-111">type</span></span>|<span data-ttu-id="2d8b7-112">String</span><span class="sxs-lookup"><span data-stu-id="2d8b7-112">String</span></span>|<span data-ttu-id="2d8b7-113">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="2d8b7-113">Actor Type.</span></span>|
|<span data-ttu-id="2d8b7-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="2d8b7-114">userPermissions</span></span>|<span data-ttu-id="2d8b7-115">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d8b7-115">String collection</span></span>|<span data-ttu-id="2d8b7-116">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="2d8b7-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="2d8b7-117">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="2d8b7-117">applicationId</span></span>|<span data-ttu-id="2d8b7-118">String</span><span class="sxs-lookup"><span data-stu-id="2d8b7-118">String</span></span>|<span data-ttu-id="2d8b7-119">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="2d8b7-119">AAD Application Id.</span></span>|
|<span data-ttu-id="2d8b7-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="2d8b7-120">applicationDisplayName</span></span>|<span data-ttu-id="2d8b7-121">String</span><span class="sxs-lookup"><span data-stu-id="2d8b7-121">String</span></span>|<span data-ttu-id="2d8b7-122">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d8b7-122">Name of the Application.</span></span>|
|<span data-ttu-id="2d8b7-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2d8b7-123">userPrincipalName</span></span>|<span data-ttu-id="2d8b7-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d8b7-124">String</span></span>|<span data-ttu-id="2d8b7-125">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="2d8b7-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="2d8b7-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="2d8b7-126">servicePrincipalName</span></span>|<span data-ttu-id="2d8b7-127">String</span><span class="sxs-lookup"><span data-stu-id="2d8b7-127">String</span></span>|<span data-ttu-id="2d8b7-128">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="2d8b7-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="2d8b7-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="2d8b7-129">ipAddress</span></span>|<span data-ttu-id="2d8b7-130">String</span><span class="sxs-lookup"><span data-stu-id="2d8b7-130">String</span></span>|<span data-ttu-id="2d8b7-131">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="2d8b7-131">IPAddress.</span></span>|
|<span data-ttu-id="2d8b7-132">userId</span><span class="sxs-lookup"><span data-stu-id="2d8b7-132">userId</span></span>|<span data-ttu-id="2d8b7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d8b7-133">String</span></span>|<span data-ttu-id="2d8b7-134">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="2d8b7-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d8b7-135">Relações</span><span class="sxs-lookup"><span data-stu-id="2d8b7-135">Relationships</span></span>
<span data-ttu-id="2d8b7-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d8b7-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d8b7-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d8b7-137">JSON Representation</span></span>
<span data-ttu-id="2d8b7-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d8b7-138">Here is a JSON representation of the resource.</span></span>
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




