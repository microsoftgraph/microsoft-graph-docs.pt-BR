---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f7d93f3a14f3f6fd1515de9232d26718b7ec0af6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971428"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="2d188-103">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="2d188-103">auditActor resource type</span></span>

> <span data-ttu-id="2d188-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2d188-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d188-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2d188-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2d188-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2d188-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d188-107">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="2d188-107">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="2d188-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d188-108">Properties</span></span>
|<span data-ttu-id="2d188-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d188-109">Property</span></span>|<span data-ttu-id="2d188-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d188-110">Type</span></span>|<span data-ttu-id="2d188-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d188-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d188-112">type</span><span class="sxs-lookup"><span data-stu-id="2d188-112">type</span></span>|<span data-ttu-id="2d188-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d188-113">String</span></span>|<span data-ttu-id="2d188-114">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="2d188-114">Actor Type.</span></span>|
|<span data-ttu-id="2d188-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="2d188-115">userPermissions</span></span>|<span data-ttu-id="2d188-116">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d188-116">String collection</span></span>|<span data-ttu-id="2d188-117">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="2d188-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="2d188-118">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="2d188-118">applicationId</span></span>|<span data-ttu-id="2d188-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d188-119">String</span></span>|<span data-ttu-id="2d188-120">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="2d188-120">AAD Application Id.</span></span>|
|<span data-ttu-id="2d188-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="2d188-121">applicationDisplayName</span></span>|<span data-ttu-id="2d188-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d188-122">String</span></span>|<span data-ttu-id="2d188-123">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d188-123">Name of the Application.</span></span>|
|<span data-ttu-id="2d188-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2d188-124">userPrincipalName</span></span>|<span data-ttu-id="2d188-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d188-125">String</span></span>|<span data-ttu-id="2d188-126">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="2d188-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="2d188-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="2d188-127">servicePrincipalName</span></span>|<span data-ttu-id="2d188-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d188-128">String</span></span>|<span data-ttu-id="2d188-129">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="2d188-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="2d188-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="2d188-130">ipAddress</span></span>|<span data-ttu-id="2d188-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d188-131">String</span></span>|<span data-ttu-id="2d188-132">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="2d188-132">IPAddress.</span></span>|
|<span data-ttu-id="2d188-133">userId</span><span class="sxs-lookup"><span data-stu-id="2d188-133">userId</span></span>|<span data-ttu-id="2d188-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d188-134">String</span></span>|<span data-ttu-id="2d188-135">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="2d188-135">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d188-136">Relações</span><span class="sxs-lookup"><span data-stu-id="2d188-136">Relationships</span></span>
<span data-ttu-id="2d188-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d188-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2d188-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d188-138">JSON Representation</span></span>
<span data-ttu-id="2d188-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d188-139">Here is a JSON representation of the resource.</span></span>
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





