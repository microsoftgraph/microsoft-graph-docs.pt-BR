---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 87cb4219df0d1b6026bee774576324eac7255377
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335246"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="cad1c-103">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="cad1c-103">auditActor resource type</span></span>

> <span data-ttu-id="cad1c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cad1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cad1c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cad1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cad1c-106">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="cad1c-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="cad1c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cad1c-107">Properties</span></span>
|<span data-ttu-id="cad1c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cad1c-108">Property</span></span>|<span data-ttu-id="cad1c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="cad1c-109">Type</span></span>|<span data-ttu-id="cad1c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cad1c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cad1c-111">type</span><span class="sxs-lookup"><span data-stu-id="cad1c-111">type</span></span>|<span data-ttu-id="cad1c-112">String</span><span class="sxs-lookup"><span data-stu-id="cad1c-112">String</span></span>|<span data-ttu-id="cad1c-113">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="cad1c-113">Actor Type.</span></span>|
|<span data-ttu-id="cad1c-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="cad1c-114">userPermissions</span></span>|<span data-ttu-id="cad1c-115">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cad1c-115">String collection</span></span>|<span data-ttu-id="cad1c-116">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="cad1c-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="cad1c-117">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="cad1c-117">applicationId</span></span>|<span data-ttu-id="cad1c-118">String</span><span class="sxs-lookup"><span data-stu-id="cad1c-118">String</span></span>|<span data-ttu-id="cad1c-119">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="cad1c-119">AAD Application Id.</span></span>|
|<span data-ttu-id="cad1c-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="cad1c-120">applicationDisplayName</span></span>|<span data-ttu-id="cad1c-121">String</span><span class="sxs-lookup"><span data-stu-id="cad1c-121">String</span></span>|<span data-ttu-id="cad1c-122">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cad1c-122">Name of the Application.</span></span>|
|<span data-ttu-id="cad1c-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cad1c-123">userPrincipalName</span></span>|<span data-ttu-id="cad1c-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cad1c-124">String</span></span>|<span data-ttu-id="cad1c-125">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="cad1c-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="cad1c-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="cad1c-126">servicePrincipalName</span></span>|<span data-ttu-id="cad1c-127">String</span><span class="sxs-lookup"><span data-stu-id="cad1c-127">String</span></span>|<span data-ttu-id="cad1c-128">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="cad1c-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="cad1c-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="cad1c-129">ipAddress</span></span>|<span data-ttu-id="cad1c-130">String</span><span class="sxs-lookup"><span data-stu-id="cad1c-130">String</span></span>|<span data-ttu-id="cad1c-131">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="cad1c-131">IPAddress.</span></span>|
|<span data-ttu-id="cad1c-132">userId</span><span class="sxs-lookup"><span data-stu-id="cad1c-132">userId</span></span>|<span data-ttu-id="cad1c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cad1c-133">String</span></span>|<span data-ttu-id="cad1c-134">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="cad1c-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cad1c-135">Relações</span><span class="sxs-lookup"><span data-stu-id="cad1c-135">Relationships</span></span>
<span data-ttu-id="cad1c-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cad1c-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cad1c-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cad1c-137">JSON Representation</span></span>
<span data-ttu-id="cad1c-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cad1c-138">Here is a JSON representation of the resource.</span></span>
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



