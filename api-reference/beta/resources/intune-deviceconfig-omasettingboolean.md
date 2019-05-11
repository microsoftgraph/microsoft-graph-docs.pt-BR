---
title: Tipo de recurso omaSettingBoolean
description: Definição booliana para configurações de OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab28f26ee4898b3481ae7f24516a650a5fea414f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950925"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="89a12-103">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="89a12-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="89a12-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89a12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89a12-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89a12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89a12-106">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="89a12-106">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="89a12-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="89a12-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="89a12-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89a12-108">Properties</span></span>
|<span data-ttu-id="89a12-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89a12-109">Property</span></span>|<span data-ttu-id="89a12-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="89a12-110">Type</span></span>|<span data-ttu-id="89a12-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="89a12-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89a12-112">displayName</span><span class="sxs-lookup"><span data-stu-id="89a12-112">displayName</span></span>|<span data-ttu-id="89a12-113">String</span><span class="sxs-lookup"><span data-stu-id="89a12-113">String</span></span>|<span data-ttu-id="89a12-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="89a12-114">Display Name.</span></span> <span data-ttu-id="89a12-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="89a12-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="89a12-116">description</span><span class="sxs-lookup"><span data-stu-id="89a12-116">description</span></span>|<span data-ttu-id="89a12-117">String</span><span class="sxs-lookup"><span data-stu-id="89a12-117">String</span></span>|<span data-ttu-id="89a12-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="89a12-118">Description.</span></span> <span data-ttu-id="89a12-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="89a12-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="89a12-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="89a12-120">omaUri</span></span>|<span data-ttu-id="89a12-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89a12-121">String</span></span>|<span data-ttu-id="89a12-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="89a12-122">OMA.</span></span> <span data-ttu-id="89a12-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="89a12-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="89a12-124">value</span><span class="sxs-lookup"><span data-stu-id="89a12-124">value</span></span>|<span data-ttu-id="89a12-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="89a12-125">Boolean</span></span>|<span data-ttu-id="89a12-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="89a12-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89a12-127">Relações</span><span class="sxs-lookup"><span data-stu-id="89a12-127">Relationships</span></span>
<span data-ttu-id="89a12-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89a12-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89a12-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89a12-129">JSON Representation</span></span>
<span data-ttu-id="89a12-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89a12-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```




