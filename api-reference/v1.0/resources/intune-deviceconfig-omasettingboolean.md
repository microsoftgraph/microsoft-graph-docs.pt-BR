---
title: Tipo de recurso omaSettingBoolean
description: Definição booliana para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3674e9d7efb438f5afb18e6fdb5b46a261086236
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760241"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="fd130-103">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="fd130-103">omaSettingBoolean resource type</span></span>

<span data-ttu-id="fd130-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd130-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd130-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fd130-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd130-106">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="fd130-106">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="fd130-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fd130-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fd130-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd130-108">Properties</span></span>
|<span data-ttu-id="fd130-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd130-109">Property</span></span>|<span data-ttu-id="fd130-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd130-110">Type</span></span>|<span data-ttu-id="fd130-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd130-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd130-112">displayName</span><span class="sxs-lookup"><span data-stu-id="fd130-112">displayName</span></span>|<span data-ttu-id="fd130-113">String</span><span class="sxs-lookup"><span data-stu-id="fd130-113">String</span></span>|<span data-ttu-id="fd130-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="fd130-114">Display Name.</span></span> <span data-ttu-id="fd130-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fd130-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fd130-116">description</span><span class="sxs-lookup"><span data-stu-id="fd130-116">description</span></span>|<span data-ttu-id="fd130-117">String</span><span class="sxs-lookup"><span data-stu-id="fd130-117">String</span></span>|<span data-ttu-id="fd130-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="fd130-118">Description.</span></span> <span data-ttu-id="fd130-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fd130-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fd130-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="fd130-120">omaUri</span></span>|<span data-ttu-id="fd130-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd130-121">String</span></span>|<span data-ttu-id="fd130-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="fd130-122">OMA.</span></span> <span data-ttu-id="fd130-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fd130-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fd130-124">value</span><span class="sxs-lookup"><span data-stu-id="fd130-124">value</span></span>|<span data-ttu-id="fd130-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd130-125">Boolean</span></span>|<span data-ttu-id="fd130-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="fd130-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd130-127">Relações</span><span class="sxs-lookup"><span data-stu-id="fd130-127">Relationships</span></span>
<span data-ttu-id="fd130-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fd130-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd130-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd130-129">JSON Representation</span></span>
<span data-ttu-id="fd130-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fd130-130">Here is a JSON representation of the resource.</span></span>
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




