---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54eec27cf91bb1da7790ae1432452ac026bf1683
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781922"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="4eb86-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="4eb86-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="4eb86-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4eb86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4eb86-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4eb86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4eb86-106">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="4eb86-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="4eb86-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4eb86-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4eb86-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4eb86-108">Properties</span></span>
|<span data-ttu-id="4eb86-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4eb86-109">Property</span></span>|<span data-ttu-id="4eb86-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4eb86-110">Type</span></span>|<span data-ttu-id="4eb86-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4eb86-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eb86-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4eb86-112">displayName</span></span>|<span data-ttu-id="4eb86-113">String</span><span class="sxs-lookup"><span data-stu-id="4eb86-113">String</span></span>|<span data-ttu-id="4eb86-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="4eb86-114">Display Name.</span></span> <span data-ttu-id="4eb86-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4eb86-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4eb86-116">description</span><span class="sxs-lookup"><span data-stu-id="4eb86-116">description</span></span>|<span data-ttu-id="4eb86-117">String</span><span class="sxs-lookup"><span data-stu-id="4eb86-117">String</span></span>|<span data-ttu-id="4eb86-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="4eb86-118">Description.</span></span> <span data-ttu-id="4eb86-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4eb86-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4eb86-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="4eb86-120">omaUri</span></span>|<span data-ttu-id="4eb86-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4eb86-121">String</span></span>|<span data-ttu-id="4eb86-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="4eb86-122">OMA.</span></span> <span data-ttu-id="4eb86-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4eb86-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4eb86-124">valor</span><span class="sxs-lookup"><span data-stu-id="4eb86-124">value</span></span>|<span data-ttu-id="4eb86-125">Int32</span><span class="sxs-lookup"><span data-stu-id="4eb86-125">Int32</span></span>|<span data-ttu-id="4eb86-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="4eb86-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4eb86-127">Relações</span><span class="sxs-lookup"><span data-stu-id="4eb86-127">Relationships</span></span>
<span data-ttu-id="4eb86-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="4eb86-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4eb86-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4eb86-129">JSON Representation</span></span>
<span data-ttu-id="4eb86-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4eb86-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```





