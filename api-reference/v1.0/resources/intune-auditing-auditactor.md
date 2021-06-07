---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ab8fc9f78fc647c82be80105cb3547e6a7a45f7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755220"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="5c8b5-103">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="5c8b5-103">auditActor resource type</span></span>

<span data-ttu-id="5c8b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c8b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c8b5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c8b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c8b5-106">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="5c8b5-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="5c8b5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5c8b5-107">Properties</span></span>
|<span data-ttu-id="5c8b5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c8b5-108">Property</span></span>|<span data-ttu-id="5c8b5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c8b5-109">Type</span></span>|<span data-ttu-id="5c8b5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c8b5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c8b5-111">tipo</span><span class="sxs-lookup"><span data-stu-id="5c8b5-111">type</span></span>|<span data-ttu-id="5c8b5-112">String</span><span class="sxs-lookup"><span data-stu-id="5c8b5-112">String</span></span>|<span data-ttu-id="5c8b5-113">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="5c8b5-113">Actor Type.</span></span>|
|<span data-ttu-id="5c8b5-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="5c8b5-114">userPermissions</span></span>|<span data-ttu-id="5c8b5-115">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c8b5-115">String collection</span></span>|<span data-ttu-id="5c8b5-116">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="5c8b5-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="5c8b5-117">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="5c8b5-117">applicationId</span></span>|<span data-ttu-id="5c8b5-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c8b5-118">String</span></span>|<span data-ttu-id="5c8b5-119">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="5c8b5-119">AAD Application Id.</span></span>|
|<span data-ttu-id="5c8b5-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="5c8b5-120">applicationDisplayName</span></span>|<span data-ttu-id="5c8b5-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c8b5-121">String</span></span>|<span data-ttu-id="5c8b5-122">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5c8b5-122">Name of the Application.</span></span>|
|<span data-ttu-id="5c8b5-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5c8b5-123">userPrincipalName</span></span>|<span data-ttu-id="5c8b5-124">String</span><span class="sxs-lookup"><span data-stu-id="5c8b5-124">String</span></span>|<span data-ttu-id="5c8b5-125">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="5c8b5-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="5c8b5-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="5c8b5-126">servicePrincipalName</span></span>|<span data-ttu-id="5c8b5-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c8b5-127">String</span></span>|<span data-ttu-id="5c8b5-128">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="5c8b5-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="5c8b5-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="5c8b5-129">ipAddress</span></span>|<span data-ttu-id="5c8b5-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c8b5-130">String</span></span>|<span data-ttu-id="5c8b5-131">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="5c8b5-131">IPAddress.</span></span>|
|<span data-ttu-id="5c8b5-132">userId</span><span class="sxs-lookup"><span data-stu-id="5c8b5-132">userId</span></span>|<span data-ttu-id="5c8b5-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c8b5-133">String</span></span>|<span data-ttu-id="5c8b5-134">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="5c8b5-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c8b5-135">Relações</span><span class="sxs-lookup"><span data-stu-id="5c8b5-135">Relationships</span></span>
<span data-ttu-id="5c8b5-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5c8b5-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c8b5-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5c8b5-137">JSON Representation</span></span>
<span data-ttu-id="5c8b5-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5c8b5-138">Here is a JSON representation of the resource.</span></span>
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




