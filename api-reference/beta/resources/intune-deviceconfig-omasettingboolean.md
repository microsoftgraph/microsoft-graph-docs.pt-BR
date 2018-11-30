---
title: Tipo de recurso omaSettingBoolean
description: Definição booliana para configurações de OMA.
ms.openlocfilehash: 2f2f156dba23fdba0f11667bf6d0c107e3cf74b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034507"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="109bb-103">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="109bb-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="109bb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="109bb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="109bb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="109bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="109bb-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="109bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="109bb-107">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="109bb-107">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="109bb-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="109bb-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="109bb-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="109bb-109">Properties</span></span>
|<span data-ttu-id="109bb-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="109bb-110">Property</span></span>|<span data-ttu-id="109bb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="109bb-111">Type</span></span>|<span data-ttu-id="109bb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="109bb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="109bb-113">displayName</span><span class="sxs-lookup"><span data-stu-id="109bb-113">displayName</span></span>|<span data-ttu-id="109bb-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="109bb-114">String</span></span>|<span data-ttu-id="109bb-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="109bb-115">Display Name.</span></span> <span data-ttu-id="109bb-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="109bb-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="109bb-117">descrição</span><span class="sxs-lookup"><span data-stu-id="109bb-117">description</span></span>|<span data-ttu-id="109bb-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="109bb-118">String</span></span>|<span data-ttu-id="109bb-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="109bb-119">Description.</span></span> <span data-ttu-id="109bb-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="109bb-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="109bb-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="109bb-121">omaUri</span></span>|<span data-ttu-id="109bb-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="109bb-122">String</span></span>|<span data-ttu-id="109bb-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="109bb-123">OMA.</span></span> <span data-ttu-id="109bb-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="109bb-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="109bb-125">valor</span><span class="sxs-lookup"><span data-stu-id="109bb-125">value</span></span>|<span data-ttu-id="109bb-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="109bb-126">Boolean</span></span>|<span data-ttu-id="109bb-127">Valor.</span><span class="sxs-lookup"><span data-stu-id="109bb-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="109bb-128">Relações</span><span class="sxs-lookup"><span data-stu-id="109bb-128">Relationships</span></span>
<span data-ttu-id="109bb-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="109bb-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="109bb-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="109bb-130">JSON Representation</span></span>
<span data-ttu-id="109bb-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="109bb-131">Here is a JSON representation of the resource.</span></span>
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





