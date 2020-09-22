---
title: Tipo de recurso omaSettingBoolean
description: Definição booliana para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a4b93559175ce44559dc3e0ad6cc0d9e71d336fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993774"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="58796-103">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="58796-103">omaSettingBoolean resource type</span></span>

<span data-ttu-id="58796-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58796-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58796-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="58796-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58796-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58796-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58796-107">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="58796-107">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="58796-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="58796-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="58796-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58796-109">Properties</span></span>
|<span data-ttu-id="58796-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58796-110">Property</span></span>|<span data-ttu-id="58796-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="58796-111">Type</span></span>|<span data-ttu-id="58796-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="58796-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58796-113">displayName</span><span class="sxs-lookup"><span data-stu-id="58796-113">displayName</span></span>|<span data-ttu-id="58796-114">String</span><span class="sxs-lookup"><span data-stu-id="58796-114">String</span></span>|<span data-ttu-id="58796-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="58796-115">Display Name.</span></span> <span data-ttu-id="58796-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="58796-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="58796-117">description</span><span class="sxs-lookup"><span data-stu-id="58796-117">description</span></span>|<span data-ttu-id="58796-118">String</span><span class="sxs-lookup"><span data-stu-id="58796-118">String</span></span>|<span data-ttu-id="58796-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="58796-119">Description.</span></span> <span data-ttu-id="58796-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="58796-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="58796-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="58796-121">omaUri</span></span>|<span data-ttu-id="58796-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58796-122">String</span></span>|<span data-ttu-id="58796-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="58796-123">OMA.</span></span> <span data-ttu-id="58796-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="58796-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="58796-125">value</span><span class="sxs-lookup"><span data-stu-id="58796-125">value</span></span>|<span data-ttu-id="58796-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="58796-126">Boolean</span></span>|<span data-ttu-id="58796-127">Valor.</span><span class="sxs-lookup"><span data-stu-id="58796-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58796-128">Relações</span><span class="sxs-lookup"><span data-stu-id="58796-128">Relationships</span></span>
<span data-ttu-id="58796-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58796-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58796-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58796-130">JSON Representation</span></span>
<span data-ttu-id="58796-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="58796-131">Here is a JSON representation of the resource.</span></span>
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






