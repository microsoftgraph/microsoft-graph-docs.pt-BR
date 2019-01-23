---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fcb9ededd9d1a2bb93f970f9f0da0c41a248e840
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425796"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="b91aa-103">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="b91aa-103">auditActor resource type</span></span>

> <span data-ttu-id="b91aa-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b91aa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b91aa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b91aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b91aa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b91aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b91aa-107">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="b91aa-107">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="b91aa-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b91aa-108">Properties</span></span>
|<span data-ttu-id="b91aa-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b91aa-109">Property</span></span>|<span data-ttu-id="b91aa-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b91aa-110">Type</span></span>|<span data-ttu-id="b91aa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b91aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b91aa-112">type</span><span class="sxs-lookup"><span data-stu-id="b91aa-112">type</span></span>|<span data-ttu-id="b91aa-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b91aa-113">String</span></span>|<span data-ttu-id="b91aa-114">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="b91aa-114">Actor Type.</span></span>|
|<span data-ttu-id="b91aa-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="b91aa-115">userPermissions</span></span>|<span data-ttu-id="b91aa-116">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b91aa-116">String collection</span></span>|<span data-ttu-id="b91aa-117">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="b91aa-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="b91aa-118">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="b91aa-118">applicationId</span></span>|<span data-ttu-id="b91aa-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b91aa-119">String</span></span>|<span data-ttu-id="b91aa-120">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="b91aa-120">AAD Application Id.</span></span>|
|<span data-ttu-id="b91aa-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="b91aa-121">applicationDisplayName</span></span>|<span data-ttu-id="b91aa-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b91aa-122">String</span></span>|<span data-ttu-id="b91aa-123">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b91aa-123">Name of the Application.</span></span>|
|<span data-ttu-id="b91aa-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b91aa-124">userPrincipalName</span></span>|<span data-ttu-id="b91aa-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b91aa-125">String</span></span>|<span data-ttu-id="b91aa-126">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="b91aa-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="b91aa-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="b91aa-127">servicePrincipalName</span></span>|<span data-ttu-id="b91aa-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b91aa-128">String</span></span>|<span data-ttu-id="b91aa-129">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="b91aa-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="b91aa-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="b91aa-130">ipAddress</span></span>|<span data-ttu-id="b91aa-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b91aa-131">String</span></span>|<span data-ttu-id="b91aa-132">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="b91aa-132">IPAddress.</span></span>|
|<span data-ttu-id="b91aa-133">userId</span><span class="sxs-lookup"><span data-stu-id="b91aa-133">userId</span></span>|<span data-ttu-id="b91aa-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b91aa-134">String</span></span>|<span data-ttu-id="b91aa-135">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="b91aa-135">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b91aa-136">Relações</span><span class="sxs-lookup"><span data-stu-id="b91aa-136">Relationships</span></span>
<span data-ttu-id="b91aa-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b91aa-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b91aa-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b91aa-138">JSON Representation</span></span>
<span data-ttu-id="b91aa-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b91aa-139">Here is a JSON representation of the resource.</span></span>
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




