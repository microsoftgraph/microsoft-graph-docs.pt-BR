---
title: Tipo de recurso omaSettingString
description: Definição de cadeia de caracteres para configurações de OMA.
author: tfitzmac
ms.openlocfilehash: a62f6dee2bf0f5a9ca96488625a84ceef5f7c785
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311197"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="05ed2-103">Tipo de recurso omaSettingString</span><span class="sxs-lookup"><span data-stu-id="05ed2-103">omaSettingString resource type</span></span>

> <span data-ttu-id="05ed2-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="05ed2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05ed2-105">Definição de cadeia de caracteres para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="05ed2-105">OMA Settings String definition.</span></span>

<span data-ttu-id="05ed2-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="05ed2-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="05ed2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05ed2-107">Properties</span></span>
|<span data-ttu-id="05ed2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05ed2-108">Property</span></span>|<span data-ttu-id="05ed2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="05ed2-109">Type</span></span>|<span data-ttu-id="05ed2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="05ed2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05ed2-111">displayName</span><span class="sxs-lookup"><span data-stu-id="05ed2-111">displayName</span></span>|<span data-ttu-id="05ed2-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05ed2-112">String</span></span>|<span data-ttu-id="05ed2-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="05ed2-113">Display Name.</span></span> <span data-ttu-id="05ed2-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="05ed2-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="05ed2-115">descrição</span><span class="sxs-lookup"><span data-stu-id="05ed2-115">description</span></span>|<span data-ttu-id="05ed2-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05ed2-116">String</span></span>|<span data-ttu-id="05ed2-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="05ed2-117">Description.</span></span> <span data-ttu-id="05ed2-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="05ed2-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="05ed2-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="05ed2-119">omaUri</span></span>|<span data-ttu-id="05ed2-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05ed2-120">String</span></span>|<span data-ttu-id="05ed2-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="05ed2-121">OMA.</span></span> <span data-ttu-id="05ed2-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="05ed2-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="05ed2-123">valor</span><span class="sxs-lookup"><span data-stu-id="05ed2-123">value</span></span>|<span data-ttu-id="05ed2-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05ed2-124">String</span></span>|<span data-ttu-id="05ed2-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="05ed2-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05ed2-126">Relações</span><span class="sxs-lookup"><span data-stu-id="05ed2-126">Relationships</span></span>
<span data-ttu-id="05ed2-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="05ed2-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="05ed2-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05ed2-128">JSON Representation</span></span>
<span data-ttu-id="05ed2-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="05ed2-129">Here is a JSON representation of the resource.</span></span>
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



