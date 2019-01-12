---
title: tipo de recurso de windowsManagementApp
description: Entidade de aplicativo de gerenciamento do Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 395148d4c870193d75f418d7dc30d2b2241bad01
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913496"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="28439-103">tipo de recurso de windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="28439-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="28439-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="28439-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28439-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="28439-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28439-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="28439-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28439-107">Entidade de aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="28439-107">Windows management app entity.</span></span>
## <a name="methods"></a><span data-ttu-id="28439-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="28439-108">Methods</span></span>
|<span data-ttu-id="28439-109">Método</span><span class="sxs-lookup"><span data-stu-id="28439-109">Method</span></span>|<span data-ttu-id="28439-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="28439-110">Return Type</span></span>|<span data-ttu-id="28439-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="28439-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="28439-112">Obter windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="28439-112">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="28439-113">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="28439-113">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="28439-114">Leia as propriedades e os relacionamentos do objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="28439-114">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="28439-115">Atualizar windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="28439-115">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="28439-116">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="28439-116">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="28439-117">Atualize as propriedades de um objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="28439-117">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="28439-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28439-118">Properties</span></span>
|<span data-ttu-id="28439-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28439-119">Property</span></span>|<span data-ttu-id="28439-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="28439-120">Type</span></span>|<span data-ttu-id="28439-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="28439-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28439-122">id</span><span class="sxs-lookup"><span data-stu-id="28439-122">id</span></span>|<span data-ttu-id="28439-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28439-123">String</span></span>|<span data-ttu-id="28439-124">Identificador exclusivo para o aplicativo de gerenciamento do Windows</span><span class="sxs-lookup"><span data-stu-id="28439-124">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="28439-125">availableVersion</span><span class="sxs-lookup"><span data-stu-id="28439-125">availableVersion</span></span>|<span data-ttu-id="28439-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28439-126">String</span></span>|<span data-ttu-id="28439-127">Versão disponível do Windows management app.</span><span class="sxs-lookup"><span data-stu-id="28439-127">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28439-128">Relações</span><span class="sxs-lookup"><span data-stu-id="28439-128">Relationships</span></span>
|<span data-ttu-id="28439-129">Relação</span><span class="sxs-lookup"><span data-stu-id="28439-129">Relationship</span></span>|<span data-ttu-id="28439-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="28439-130">Type</span></span>|<span data-ttu-id="28439-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="28439-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28439-132">healthSummary</span><span class="sxs-lookup"><span data-stu-id="28439-132">healthSummary</span></span>|[<span data-ttu-id="28439-133">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="28439-133">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="28439-134">Integridade de resumida de aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="28439-134">Health summary for Windows management app.</span></span>|
|<span data-ttu-id="28439-135">healthStates</span><span class="sxs-lookup"><span data-stu-id="28439-135">healthStates</span></span>|<span data-ttu-id="28439-136">coleção [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)</span><span class="sxs-lookup"><span data-stu-id="28439-136">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="28439-137">A lista de estados de integridade para o aplicativo de gerenciamento do Windows instalado.</span><span class="sxs-lookup"><span data-stu-id="28439-137">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28439-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28439-138">JSON Representation</span></span>
<span data-ttu-id="28439-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28439-139">Here is a JSON representation of the resource.</span></span>
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





