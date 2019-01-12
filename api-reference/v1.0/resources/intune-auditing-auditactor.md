---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ba63fd04d917a464933e749622a5abf959c2859e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948699"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="6e4c3-103">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="6e4c3-103">auditActor resource type</span></span>

> <span data-ttu-id="6e4c3-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6e4c3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e4c3-105">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="6e4c3-105">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="6e4c3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e4c3-106">Properties</span></span>
|<span data-ttu-id="6e4c3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e4c3-107">Property</span></span>|<span data-ttu-id="6e4c3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e4c3-108">Type</span></span>|<span data-ttu-id="6e4c3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e4c3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e4c3-110">type</span><span class="sxs-lookup"><span data-stu-id="6e4c3-110">type</span></span>|<span data-ttu-id="6e4c3-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e4c3-111">String</span></span>|<span data-ttu-id="6e4c3-112">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="6e4c3-112">Actor Type.</span></span>|
|<span data-ttu-id="6e4c3-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="6e4c3-113">userPermissions</span></span>|<span data-ttu-id="6e4c3-114">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e4c3-114">String collection</span></span>|<span data-ttu-id="6e4c3-115">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="6e4c3-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="6e4c3-116">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="6e4c3-116">applicationId</span></span>|<span data-ttu-id="6e4c3-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e4c3-117">String</span></span>|<span data-ttu-id="6e4c3-118">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="6e4c3-118">AAD Application Id.</span></span>|
|<span data-ttu-id="6e4c3-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="6e4c3-119">applicationDisplayName</span></span>|<span data-ttu-id="6e4c3-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e4c3-120">String</span></span>|<span data-ttu-id="6e4c3-121">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6e4c3-121">Name of the Application.</span></span>|
|<span data-ttu-id="6e4c3-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6e4c3-122">userPrincipalName</span></span>|<span data-ttu-id="6e4c3-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e4c3-123">String</span></span>|<span data-ttu-id="6e4c3-124">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="6e4c3-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="6e4c3-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="6e4c3-125">servicePrincipalName</span></span>|<span data-ttu-id="6e4c3-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e4c3-126">String</span></span>|<span data-ttu-id="6e4c3-127">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="6e4c3-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="6e4c3-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="6e4c3-128">ipAddress</span></span>|<span data-ttu-id="6e4c3-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e4c3-129">String</span></span>|<span data-ttu-id="6e4c3-130">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="6e4c3-130">IPAddress.</span></span>|
|<span data-ttu-id="6e4c3-131">userId</span><span class="sxs-lookup"><span data-stu-id="6e4c3-131">userId</span></span>|<span data-ttu-id="6e4c3-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e4c3-132">String</span></span>|<span data-ttu-id="6e4c3-133">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="6e4c3-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e4c3-134">Relações</span><span class="sxs-lookup"><span data-stu-id="6e4c3-134">Relationships</span></span>
<span data-ttu-id="6e4c3-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e4c3-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6e4c3-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e4c3-136">JSON Representation</span></span>
<span data-ttu-id="6e4c3-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e4c3-137">Here is a JSON representation of the resource.</span></span>
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



