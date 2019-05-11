---
title: Tipo de recurso omaSettingString
description: Definição de cadeia de caracteres para configurações de OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53840e360446975dcbe6fda170ea26892fce3983
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950946"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="86944-103">Tipo de recurso omaSettingString</span><span class="sxs-lookup"><span data-stu-id="86944-103">omaSettingString resource type</span></span>

> <span data-ttu-id="86944-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86944-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86944-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86944-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86944-106">Definição de cadeia de caracteres para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="86944-106">OMA Settings String definition.</span></span>


<span data-ttu-id="86944-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="86944-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="86944-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86944-108">Properties</span></span>
|<span data-ttu-id="86944-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86944-109">Property</span></span>|<span data-ttu-id="86944-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="86944-110">Type</span></span>|<span data-ttu-id="86944-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="86944-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86944-112">displayName</span><span class="sxs-lookup"><span data-stu-id="86944-112">displayName</span></span>|<span data-ttu-id="86944-113">String</span><span class="sxs-lookup"><span data-stu-id="86944-113">String</span></span>|<span data-ttu-id="86944-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="86944-114">Display Name.</span></span> <span data-ttu-id="86944-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="86944-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="86944-116">description</span><span class="sxs-lookup"><span data-stu-id="86944-116">description</span></span>|<span data-ttu-id="86944-117">String</span><span class="sxs-lookup"><span data-stu-id="86944-117">String</span></span>|<span data-ttu-id="86944-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="86944-118">Description.</span></span> <span data-ttu-id="86944-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="86944-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="86944-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="86944-120">omaUri</span></span>|<span data-ttu-id="86944-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86944-121">String</span></span>|<span data-ttu-id="86944-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="86944-122">OMA.</span></span> <span data-ttu-id="86944-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="86944-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="86944-124">value</span><span class="sxs-lookup"><span data-stu-id="86944-124">value</span></span>|<span data-ttu-id="86944-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86944-125">String</span></span>|<span data-ttu-id="86944-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="86944-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86944-127">Relações</span><span class="sxs-lookup"><span data-stu-id="86944-127">Relationships</span></span>
<span data-ttu-id="86944-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="86944-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86944-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86944-129">JSON Representation</span></span>
<span data-ttu-id="86944-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86944-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```




