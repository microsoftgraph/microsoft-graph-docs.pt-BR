---
title: Tipo de recurso omaSettingBoolean
description: Definição booliana para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d202997cdf0c1325e887337842513cc30dd2941
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549535"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="b2fad-103">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="b2fad-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="b2fad-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2fad-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2fad-105">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="b2fad-105">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="b2fad-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b2fad-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b2fad-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2fad-107">Properties</span></span>
|<span data-ttu-id="b2fad-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2fad-108">Property</span></span>|<span data-ttu-id="b2fad-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2fad-109">Type</span></span>|<span data-ttu-id="b2fad-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2fad-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2fad-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b2fad-111">displayName</span></span>|<span data-ttu-id="b2fad-112">String</span><span class="sxs-lookup"><span data-stu-id="b2fad-112">String</span></span>|<span data-ttu-id="b2fad-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="b2fad-113">Display Name.</span></span> <span data-ttu-id="b2fad-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b2fad-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b2fad-115">description</span><span class="sxs-lookup"><span data-stu-id="b2fad-115">description</span></span>|<span data-ttu-id="b2fad-116">String</span><span class="sxs-lookup"><span data-stu-id="b2fad-116">String</span></span>|<span data-ttu-id="b2fad-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="b2fad-117">Description.</span></span> <span data-ttu-id="b2fad-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b2fad-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b2fad-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="b2fad-119">omaUri</span></span>|<span data-ttu-id="b2fad-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2fad-120">String</span></span>|<span data-ttu-id="b2fad-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="b2fad-121">OMA.</span></span> <span data-ttu-id="b2fad-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b2fad-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b2fad-123">value</span><span class="sxs-lookup"><span data-stu-id="b2fad-123">value</span></span>|<span data-ttu-id="b2fad-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2fad-124">Boolean</span></span>|<span data-ttu-id="b2fad-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="b2fad-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2fad-126">Relações</span><span class="sxs-lookup"><span data-stu-id="b2fad-126">Relationships</span></span>
<span data-ttu-id="b2fad-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2fad-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2fad-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2fad-128">JSON Representation</span></span>
<span data-ttu-id="b2fad-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b2fad-129">Here is a JSON representation of the resource.</span></span>
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



