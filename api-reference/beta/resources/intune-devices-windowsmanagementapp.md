---
title: tipo de recurso windowsManagementApp
description: Entidade do aplicativo de gerenciamento do Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4525767a81b0e69ed1c99ae4b1a20051304cf1f2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941904"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="62f55-103">tipo de recurso windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="62f55-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="62f55-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62f55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62f55-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62f55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62f55-106">Entidade do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="62f55-106">Windows management app entity.</span></span>

## <a name="methods"></a><span data-ttu-id="62f55-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="62f55-107">Methods</span></span>
|<span data-ttu-id="62f55-108">Método</span><span class="sxs-lookup"><span data-stu-id="62f55-108">Method</span></span>|<span data-ttu-id="62f55-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="62f55-109">Return Type</span></span>|<span data-ttu-id="62f55-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="62f55-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="62f55-111">Obter windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="62f55-111">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="62f55-112">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="62f55-112">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="62f55-113">Leia as propriedades e as relações do objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="62f55-113">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="62f55-114">Atualizar windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="62f55-114">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="62f55-115">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="62f55-115">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="62f55-116">Atualiza as propriedades de um objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="62f55-116">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="62f55-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62f55-117">Properties</span></span>
|<span data-ttu-id="62f55-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62f55-118">Property</span></span>|<span data-ttu-id="62f55-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="62f55-119">Type</span></span>|<span data-ttu-id="62f55-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="62f55-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62f55-121">id</span><span class="sxs-lookup"><span data-stu-id="62f55-121">id</span></span>|<span data-ttu-id="62f55-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62f55-122">String</span></span>|<span data-ttu-id="62f55-123">Identificador exclusivo para o aplicativo de gerenciamento do Windows</span><span class="sxs-lookup"><span data-stu-id="62f55-123">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="62f55-124">availableVersion</span><span class="sxs-lookup"><span data-stu-id="62f55-124">availableVersion</span></span>|<span data-ttu-id="62f55-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62f55-125">String</span></span>|<span data-ttu-id="62f55-126">Versão disponível do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="62f55-126">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62f55-127">Relações</span><span class="sxs-lookup"><span data-stu-id="62f55-127">Relationships</span></span>
|<span data-ttu-id="62f55-128">Relação</span><span class="sxs-lookup"><span data-stu-id="62f55-128">Relationship</span></span>|<span data-ttu-id="62f55-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="62f55-129">Type</span></span>|<span data-ttu-id="62f55-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="62f55-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62f55-131">healthSummary</span><span class="sxs-lookup"><span data-stu-id="62f55-131">healthSummary</span></span>|[<span data-ttu-id="62f55-132">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="62f55-132">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="62f55-133">Resumo de integridade do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="62f55-133">Health summary for Windows management app.</span></span>|
|<span data-ttu-id="62f55-134">healthStates</span><span class="sxs-lookup"><span data-stu-id="62f55-134">healthStates</span></span>|<span data-ttu-id="62f55-135">coleção [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)</span><span class="sxs-lookup"><span data-stu-id="62f55-135">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="62f55-136">A lista de Estados de integridade para o aplicativo de gerenciamento do Windows instalado.</span><span class="sxs-lookup"><span data-stu-id="62f55-136">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62f55-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62f55-137">JSON Representation</span></span>
<span data-ttu-id="62f55-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62f55-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String"
}
```




