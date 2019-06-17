---
title: Tipo de recurso omaSettingBoolean
description: Definição booliana para configurações de OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7269b8c61603601d0932a000f7f90e63d7cbc44e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993729"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="81f66-103">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="81f66-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="81f66-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81f66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81f66-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81f66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81f66-106">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="81f66-106">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="81f66-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81f66-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="81f66-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81f66-108">Properties</span></span>
|<span data-ttu-id="81f66-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81f66-109">Property</span></span>|<span data-ttu-id="81f66-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="81f66-110">Type</span></span>|<span data-ttu-id="81f66-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="81f66-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81f66-112">displayName</span><span class="sxs-lookup"><span data-stu-id="81f66-112">displayName</span></span>|<span data-ttu-id="81f66-113">String</span><span class="sxs-lookup"><span data-stu-id="81f66-113">String</span></span>|<span data-ttu-id="81f66-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="81f66-114">Display Name.</span></span> <span data-ttu-id="81f66-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81f66-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="81f66-116">descrição</span><span class="sxs-lookup"><span data-stu-id="81f66-116">description</span></span>|<span data-ttu-id="81f66-117">String</span><span class="sxs-lookup"><span data-stu-id="81f66-117">String</span></span>|<span data-ttu-id="81f66-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="81f66-118">Description.</span></span> <span data-ttu-id="81f66-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81f66-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="81f66-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="81f66-120">omaUri</span></span>|<span data-ttu-id="81f66-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81f66-121">String</span></span>|<span data-ttu-id="81f66-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="81f66-122">OMA.</span></span> <span data-ttu-id="81f66-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81f66-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="81f66-124">value</span><span class="sxs-lookup"><span data-stu-id="81f66-124">value</span></span>|<span data-ttu-id="81f66-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="81f66-125">Boolean</span></span>|<span data-ttu-id="81f66-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="81f66-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81f66-127">Relações</span><span class="sxs-lookup"><span data-stu-id="81f66-127">Relationships</span></span>
<span data-ttu-id="81f66-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81f66-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81f66-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81f66-129">JSON Representation</span></span>
<span data-ttu-id="81f66-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81f66-130">Here is a JSON representation of the resource.</span></span>
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





