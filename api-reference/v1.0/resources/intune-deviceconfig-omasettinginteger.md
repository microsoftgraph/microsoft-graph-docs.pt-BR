---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e4896af0e43510eb791f37a72a864a405388e9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569015"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="d5304-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="d5304-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="d5304-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5304-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5304-105">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="d5304-105">OMA Settings Integer definition.</span></span>


<span data-ttu-id="d5304-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d5304-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d5304-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5304-107">Properties</span></span>
|<span data-ttu-id="d5304-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5304-108">Property</span></span>|<span data-ttu-id="d5304-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5304-109">Type</span></span>|<span data-ttu-id="d5304-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5304-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5304-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d5304-111">displayName</span></span>|<span data-ttu-id="d5304-112">String</span><span class="sxs-lookup"><span data-stu-id="d5304-112">String</span></span>|<span data-ttu-id="d5304-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="d5304-113">Display Name.</span></span> <span data-ttu-id="d5304-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d5304-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d5304-115">description</span><span class="sxs-lookup"><span data-stu-id="d5304-115">description</span></span>|<span data-ttu-id="d5304-116">String</span><span class="sxs-lookup"><span data-stu-id="d5304-116">String</span></span>|<span data-ttu-id="d5304-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="d5304-117">Description.</span></span> <span data-ttu-id="d5304-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d5304-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d5304-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="d5304-119">omaUri</span></span>|<span data-ttu-id="d5304-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5304-120">String</span></span>|<span data-ttu-id="d5304-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="d5304-121">OMA.</span></span> <span data-ttu-id="d5304-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d5304-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d5304-123">valor</span><span class="sxs-lookup"><span data-stu-id="d5304-123">value</span></span>|<span data-ttu-id="d5304-124">Int32</span><span class="sxs-lookup"><span data-stu-id="d5304-124">Int32</span></span>|<span data-ttu-id="d5304-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="d5304-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5304-126">Relações</span><span class="sxs-lookup"><span data-stu-id="d5304-126">Relationships</span></span>
<span data-ttu-id="d5304-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5304-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5304-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5304-128">JSON Representation</span></span>
<span data-ttu-id="d5304-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5304-129">Here is a JSON representation of the resource.</span></span>
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



