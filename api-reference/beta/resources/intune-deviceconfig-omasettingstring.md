---
title: Tipo de recurso omaSettingString
description: Definição de cadeia de caracteres para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a22c69270126349d8d1d4afca4555abd18768aa3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566784"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="fc40e-103">Tipo de recurso omaSettingString</span><span class="sxs-lookup"><span data-stu-id="fc40e-103">omaSettingString resource type</span></span>

> <span data-ttu-id="fc40e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fc40e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc40e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc40e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc40e-106">Definição de cadeia de caracteres para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="fc40e-106">OMA Settings String definition.</span></span>


<span data-ttu-id="fc40e-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fc40e-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fc40e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc40e-108">Properties</span></span>
|<span data-ttu-id="fc40e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc40e-109">Property</span></span>|<span data-ttu-id="fc40e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc40e-110">Type</span></span>|<span data-ttu-id="fc40e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc40e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc40e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="fc40e-112">displayName</span></span>|<span data-ttu-id="fc40e-113">String</span><span class="sxs-lookup"><span data-stu-id="fc40e-113">String</span></span>|<span data-ttu-id="fc40e-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="fc40e-114">Display Name.</span></span> <span data-ttu-id="fc40e-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fc40e-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fc40e-116">description</span><span class="sxs-lookup"><span data-stu-id="fc40e-116">description</span></span>|<span data-ttu-id="fc40e-117">String</span><span class="sxs-lookup"><span data-stu-id="fc40e-117">String</span></span>|<span data-ttu-id="fc40e-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="fc40e-118">Description.</span></span> <span data-ttu-id="fc40e-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fc40e-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fc40e-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="fc40e-120">omaUri</span></span>|<span data-ttu-id="fc40e-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc40e-121">String</span></span>|<span data-ttu-id="fc40e-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="fc40e-122">OMA.</span></span> <span data-ttu-id="fc40e-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fc40e-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fc40e-124">value</span><span class="sxs-lookup"><span data-stu-id="fc40e-124">value</span></span>|<span data-ttu-id="fc40e-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc40e-125">String</span></span>|<span data-ttu-id="fc40e-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="fc40e-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc40e-127">Relações</span><span class="sxs-lookup"><span data-stu-id="fc40e-127">Relationships</span></span>
<span data-ttu-id="fc40e-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc40e-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc40e-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc40e-129">JSON Representation</span></span>
<span data-ttu-id="fc40e-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc40e-130">Here is a JSON representation of the resource.</span></span>
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





