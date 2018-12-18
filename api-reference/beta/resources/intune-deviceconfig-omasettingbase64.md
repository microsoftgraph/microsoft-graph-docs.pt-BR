---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: tfitzmac
ms.openlocfilehash: ee25db94cc1426194166a7c66b9a8a626d62c3e4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304071"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="0f9db-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="0f9db-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="0f9db-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0f9db-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f9db-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0f9db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f9db-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0f9db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f9db-107">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="0f9db-107">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="0f9db-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f9db-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f9db-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f9db-109">Properties</span></span>
|<span data-ttu-id="0f9db-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f9db-110">Property</span></span>|<span data-ttu-id="0f9db-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f9db-111">Type</span></span>|<span data-ttu-id="0f9db-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f9db-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f9db-113">displayName</span><span class="sxs-lookup"><span data-stu-id="0f9db-113">displayName</span></span>|<span data-ttu-id="0f9db-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f9db-114">String</span></span>|<span data-ttu-id="0f9db-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="0f9db-115">Display Name.</span></span> <span data-ttu-id="0f9db-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f9db-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0f9db-117">descrição</span><span class="sxs-lookup"><span data-stu-id="0f9db-117">description</span></span>|<span data-ttu-id="0f9db-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f9db-118">String</span></span>|<span data-ttu-id="0f9db-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="0f9db-119">Description.</span></span> <span data-ttu-id="0f9db-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f9db-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0f9db-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="0f9db-121">omaUri</span></span>|<span data-ttu-id="0f9db-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f9db-122">String</span></span>|<span data-ttu-id="0f9db-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="0f9db-123">OMA.</span></span> <span data-ttu-id="0f9db-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f9db-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0f9db-125">fileName</span><span class="sxs-lookup"><span data-stu-id="0f9db-125">fileName</span></span>|<span data-ttu-id="0f9db-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f9db-126">String</span></span>|<span data-ttu-id="0f9db-127">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="0f9db-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="0f9db-128">CRT</span><span class="sxs-lookup"><span data-stu-id="0f9db-128">\*.crt</span></span> | <span data-ttu-id="0f9db-129">p7b</span><span class="sxs-lookup"><span data-stu-id="0f9db-129">\*.p7b</span></span> | <span data-ttu-id="0f9db-130">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="0f9db-130">\*.bin).</span></span>|
|<span data-ttu-id="0f9db-131">valor</span><span class="sxs-lookup"><span data-stu-id="0f9db-131">value</span></span>|<span data-ttu-id="0f9db-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f9db-132">String</span></span>|<span data-ttu-id="0f9db-133">Valor.</span><span class="sxs-lookup"><span data-stu-id="0f9db-133">Value.</span></span> <span data-ttu-id="0f9db-134">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="0f9db-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f9db-135">Relações</span><span class="sxs-lookup"><span data-stu-id="0f9db-135">Relationships</span></span>
<span data-ttu-id="0f9db-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0f9db-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f9db-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f9db-137">JSON Representation</span></span>
<span data-ttu-id="0f9db-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f9db-138">Here is a JSON representation of the resource.</span></span>
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





