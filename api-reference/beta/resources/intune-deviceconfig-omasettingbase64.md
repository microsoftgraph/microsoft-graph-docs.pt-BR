---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
ms.openlocfilehash: eebe9730c36ab4bc7e48aa765ecd3959897c6c12
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036603"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="7bddc-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="7bddc-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="7bddc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7bddc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7bddc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7bddc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7bddc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7bddc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7bddc-107">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="7bddc-107">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="7bddc-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7bddc-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7bddc-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7bddc-109">Properties</span></span>
|<span data-ttu-id="7bddc-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bddc-110">Property</span></span>|<span data-ttu-id="7bddc-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bddc-111">Type</span></span>|<span data-ttu-id="7bddc-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bddc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bddc-113">displayName</span><span class="sxs-lookup"><span data-stu-id="7bddc-113">displayName</span></span>|<span data-ttu-id="7bddc-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bddc-114">String</span></span>|<span data-ttu-id="7bddc-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="7bddc-115">Display Name.</span></span> <span data-ttu-id="7bddc-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7bddc-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7bddc-117">descrição</span><span class="sxs-lookup"><span data-stu-id="7bddc-117">description</span></span>|<span data-ttu-id="7bddc-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bddc-118">String</span></span>|<span data-ttu-id="7bddc-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="7bddc-119">Description.</span></span> <span data-ttu-id="7bddc-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7bddc-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7bddc-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="7bddc-121">omaUri</span></span>|<span data-ttu-id="7bddc-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bddc-122">String</span></span>|<span data-ttu-id="7bddc-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="7bddc-123">OMA.</span></span> <span data-ttu-id="7bddc-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7bddc-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7bddc-125">fileName</span><span class="sxs-lookup"><span data-stu-id="7bddc-125">fileName</span></span>|<span data-ttu-id="7bddc-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bddc-126">String</span></span>|<span data-ttu-id="7bddc-127">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="7bddc-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="7bddc-128">CRT</span><span class="sxs-lookup"><span data-stu-id="7bddc-128">\*.crt</span></span> | <span data-ttu-id="7bddc-129">p7b</span><span class="sxs-lookup"><span data-stu-id="7bddc-129">\*.p7b</span></span> | <span data-ttu-id="7bddc-130">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="7bddc-130">\*.bin).</span></span>|
|<span data-ttu-id="7bddc-131">valor</span><span class="sxs-lookup"><span data-stu-id="7bddc-131">value</span></span>|<span data-ttu-id="7bddc-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bddc-132">String</span></span>|<span data-ttu-id="7bddc-133">Valor.</span><span class="sxs-lookup"><span data-stu-id="7bddc-133">Value.</span></span> <span data-ttu-id="7bddc-134">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="7bddc-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bddc-135">Relações</span><span class="sxs-lookup"><span data-stu-id="7bddc-135">Relationships</span></span>
<span data-ttu-id="7bddc-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7bddc-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7bddc-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7bddc-137">JSON Representation</span></span>
<span data-ttu-id="7bddc-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7bddc-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```





