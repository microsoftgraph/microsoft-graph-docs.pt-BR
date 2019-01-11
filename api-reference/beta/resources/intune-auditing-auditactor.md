---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4c6dddd2863f881c026eb848c643bdc55cbbb372
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873910"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="98eba-103">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="98eba-103">auditActor resource type</span></span>

> <span data-ttu-id="98eba-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="98eba-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98eba-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="98eba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98eba-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="98eba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98eba-107">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="98eba-107">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="98eba-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98eba-108">Properties</span></span>
|<span data-ttu-id="98eba-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98eba-109">Property</span></span>|<span data-ttu-id="98eba-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="98eba-110">Type</span></span>|<span data-ttu-id="98eba-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="98eba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98eba-112">type</span><span class="sxs-lookup"><span data-stu-id="98eba-112">type</span></span>|<span data-ttu-id="98eba-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98eba-113">String</span></span>|<span data-ttu-id="98eba-114">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="98eba-114">Actor Type.</span></span>|
|<span data-ttu-id="98eba-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="98eba-115">userPermissions</span></span>|<span data-ttu-id="98eba-116">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98eba-116">String collection</span></span>|<span data-ttu-id="98eba-117">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="98eba-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="98eba-118">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="98eba-118">applicationId</span></span>|<span data-ttu-id="98eba-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98eba-119">String</span></span>|<span data-ttu-id="98eba-120">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="98eba-120">AAD Application Id.</span></span>|
|<span data-ttu-id="98eba-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="98eba-121">applicationDisplayName</span></span>|<span data-ttu-id="98eba-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98eba-122">String</span></span>|<span data-ttu-id="98eba-123">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="98eba-123">Name of the Application.</span></span>|
|<span data-ttu-id="98eba-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="98eba-124">userPrincipalName</span></span>|<span data-ttu-id="98eba-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98eba-125">String</span></span>|<span data-ttu-id="98eba-126">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="98eba-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="98eba-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="98eba-127">servicePrincipalName</span></span>|<span data-ttu-id="98eba-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98eba-128">String</span></span>|<span data-ttu-id="98eba-129">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="98eba-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="98eba-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="98eba-130">ipAddress</span></span>|<span data-ttu-id="98eba-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98eba-131">String</span></span>|<span data-ttu-id="98eba-132">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="98eba-132">IPAddress.</span></span>|
|<span data-ttu-id="98eba-133">userId</span><span class="sxs-lookup"><span data-stu-id="98eba-133">userId</span></span>|<span data-ttu-id="98eba-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98eba-134">String</span></span>|<span data-ttu-id="98eba-135">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="98eba-135">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98eba-136">Relações</span><span class="sxs-lookup"><span data-stu-id="98eba-136">Relationships</span></span>
<span data-ttu-id="98eba-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="98eba-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="98eba-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98eba-138">JSON Representation</span></span>
<span data-ttu-id="98eba-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="98eba-139">Here is a JSON representation of the resource.</span></span>
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





