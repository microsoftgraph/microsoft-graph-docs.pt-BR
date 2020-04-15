---
title: Tipo de recurso omaSettingBoolean
description: Definição booliana para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fa56968ec1b427a20f564fa5dddafd250050fa0f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473045"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="fadce-103">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="fadce-103">omaSettingBoolean resource type</span></span>

<span data-ttu-id="fadce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fadce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fadce-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fadce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fadce-106">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="fadce-106">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="fadce-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fadce-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fadce-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fadce-108">Properties</span></span>
|<span data-ttu-id="fadce-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fadce-109">Property</span></span>|<span data-ttu-id="fadce-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fadce-110">Type</span></span>|<span data-ttu-id="fadce-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fadce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fadce-112">displayName</span><span class="sxs-lookup"><span data-stu-id="fadce-112">displayName</span></span>|<span data-ttu-id="fadce-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fadce-113">String</span></span>|<span data-ttu-id="fadce-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="fadce-114">Display Name.</span></span> <span data-ttu-id="fadce-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fadce-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fadce-116">description</span><span class="sxs-lookup"><span data-stu-id="fadce-116">description</span></span>|<span data-ttu-id="fadce-117">String</span><span class="sxs-lookup"><span data-stu-id="fadce-117">String</span></span>|<span data-ttu-id="fadce-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="fadce-118">Description.</span></span> <span data-ttu-id="fadce-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fadce-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fadce-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="fadce-120">omaUri</span></span>|<span data-ttu-id="fadce-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fadce-121">String</span></span>|<span data-ttu-id="fadce-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="fadce-122">OMA.</span></span> <span data-ttu-id="fadce-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fadce-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fadce-124">value</span><span class="sxs-lookup"><span data-stu-id="fadce-124">value</span></span>|<span data-ttu-id="fadce-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="fadce-125">Boolean</span></span>|<span data-ttu-id="fadce-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="fadce-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fadce-127">Relações</span><span class="sxs-lookup"><span data-stu-id="fadce-127">Relationships</span></span>
<span data-ttu-id="fadce-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fadce-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fadce-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fadce-129">JSON Representation</span></span>
<span data-ttu-id="fadce-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fadce-130">Here is a JSON representation of the resource.</span></span>
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







