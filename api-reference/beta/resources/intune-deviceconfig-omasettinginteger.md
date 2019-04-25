---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54eec27cf91bb1da7790ae1432452ac026bf1683
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542120"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="4a590-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="4a590-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="4a590-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4a590-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a590-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a590-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a590-106">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="4a590-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="4a590-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4a590-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4a590-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a590-108">Properties</span></span>
|<span data-ttu-id="4a590-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a590-109">Property</span></span>|<span data-ttu-id="4a590-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a590-110">Type</span></span>|<span data-ttu-id="4a590-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a590-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a590-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4a590-112">displayName</span></span>|<span data-ttu-id="4a590-113">String</span><span class="sxs-lookup"><span data-stu-id="4a590-113">String</span></span>|<span data-ttu-id="4a590-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="4a590-114">Display Name.</span></span> <span data-ttu-id="4a590-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4a590-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4a590-116">description</span><span class="sxs-lookup"><span data-stu-id="4a590-116">description</span></span>|<span data-ttu-id="4a590-117">String</span><span class="sxs-lookup"><span data-stu-id="4a590-117">String</span></span>|<span data-ttu-id="4a590-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="4a590-118">Description.</span></span> <span data-ttu-id="4a590-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4a590-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4a590-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="4a590-120">omaUri</span></span>|<span data-ttu-id="4a590-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a590-121">String</span></span>|<span data-ttu-id="4a590-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="4a590-122">OMA.</span></span> <span data-ttu-id="4a590-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4a590-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4a590-124">valor</span><span class="sxs-lookup"><span data-stu-id="4a590-124">value</span></span>|<span data-ttu-id="4a590-125">Int32</span><span class="sxs-lookup"><span data-stu-id="4a590-125">Int32</span></span>|<span data-ttu-id="4a590-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="4a590-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a590-127">Relações</span><span class="sxs-lookup"><span data-stu-id="4a590-127">Relationships</span></span>
<span data-ttu-id="4a590-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a590-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a590-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a590-129">JSON Representation</span></span>
<span data-ttu-id="4a590-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a590-130">Here is a JSON representation of the resource.</span></span>
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





