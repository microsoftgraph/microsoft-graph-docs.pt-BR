---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: tfitzmac
ms.openlocfilehash: 1b1f3a182aa710564bdf5e134a4ceabf22f3fb71
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348927"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="ef5ed-103">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="ef5ed-103">auditActor resource type</span></span>

> <span data-ttu-id="ef5ed-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ef5ed-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef5ed-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ef5ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef5ed-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ef5ed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef5ed-107">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="ef5ed-107">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="ef5ed-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef5ed-108">Properties</span></span>
|<span data-ttu-id="ef5ed-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef5ed-109">Property</span></span>|<span data-ttu-id="ef5ed-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef5ed-110">Type</span></span>|<span data-ttu-id="ef5ed-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef5ed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef5ed-112">type</span><span class="sxs-lookup"><span data-stu-id="ef5ed-112">type</span></span>|<span data-ttu-id="ef5ed-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef5ed-113">String</span></span>|<span data-ttu-id="ef5ed-114">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="ef5ed-114">Actor Type.</span></span>|
|<span data-ttu-id="ef5ed-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="ef5ed-115">userPermissions</span></span>|<span data-ttu-id="ef5ed-116">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef5ed-116">String collection</span></span>|<span data-ttu-id="ef5ed-117">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="ef5ed-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="ef5ed-118">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="ef5ed-118">applicationId</span></span>|<span data-ttu-id="ef5ed-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef5ed-119">String</span></span>|<span data-ttu-id="ef5ed-120">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="ef5ed-120">AAD Application Id.</span></span>|
|<span data-ttu-id="ef5ed-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="ef5ed-121">applicationDisplayName</span></span>|<span data-ttu-id="ef5ed-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef5ed-122">String</span></span>|<span data-ttu-id="ef5ed-123">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ef5ed-123">Name of the Application.</span></span>|
|<span data-ttu-id="ef5ed-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ef5ed-124">userPrincipalName</span></span>|<span data-ttu-id="ef5ed-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef5ed-125">String</span></span>|<span data-ttu-id="ef5ed-126">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="ef5ed-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="ef5ed-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="ef5ed-127">servicePrincipalName</span></span>|<span data-ttu-id="ef5ed-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef5ed-128">String</span></span>|<span data-ttu-id="ef5ed-129">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="ef5ed-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="ef5ed-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="ef5ed-130">ipAddress</span></span>|<span data-ttu-id="ef5ed-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef5ed-131">String</span></span>|<span data-ttu-id="ef5ed-132">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="ef5ed-132">IPAddress.</span></span>|
|<span data-ttu-id="ef5ed-133">userId</span><span class="sxs-lookup"><span data-stu-id="ef5ed-133">userId</span></span>|<span data-ttu-id="ef5ed-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef5ed-134">String</span></span>|<span data-ttu-id="ef5ed-135">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="ef5ed-135">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef5ed-136">Relações</span><span class="sxs-lookup"><span data-stu-id="ef5ed-136">Relationships</span></span>
<span data-ttu-id="ef5ed-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ef5ed-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ef5ed-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef5ed-138">JSON Representation</span></span>
<span data-ttu-id="ef5ed-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef5ed-139">Here is a JSON representation of the resource.</span></span>
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





