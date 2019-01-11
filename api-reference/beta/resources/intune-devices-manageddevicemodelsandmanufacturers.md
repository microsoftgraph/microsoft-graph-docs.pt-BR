---
title: tipo de recurso de managedDeviceModelsAndManufacturers
description: Modelos e fabricantes meatadata para dispositivos gerenciados na conta
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 86d9f9dd0642abab73f6b750b997c75851f6be02
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875618"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="87a41-103">tipo de recurso de managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="87a41-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="87a41-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="87a41-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87a41-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="87a41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87a41-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="87a41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87a41-107">Modelos e fabricantes meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="87a41-107">Models and Manufactures meatadata for managed devices in the account</span></span>
## <a name="properties"></a><span data-ttu-id="87a41-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87a41-108">Properties</span></span>
|<span data-ttu-id="87a41-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87a41-109">Property</span></span>|<span data-ttu-id="87a41-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="87a41-110">Type</span></span>|<span data-ttu-id="87a41-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="87a41-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87a41-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="87a41-112">deviceModels</span></span>|<span data-ttu-id="87a41-113">String collection</span><span class="sxs-lookup"><span data-stu-id="87a41-113">String collection</span></span>|<span data-ttu-id="87a41-114">Lista de modelos para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="87a41-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="87a41-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="87a41-115">deviceManufacturers</span></span>|<span data-ttu-id="87a41-116">String collection</span><span class="sxs-lookup"><span data-stu-id="87a41-116">String collection</span></span>|<span data-ttu-id="87a41-117">Lista de fabricantes de dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="87a41-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="87a41-118">Relações</span><span class="sxs-lookup"><span data-stu-id="87a41-118">Relationships</span></span>
<span data-ttu-id="87a41-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87a41-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="87a41-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87a41-120">JSON Representation</span></span>
<span data-ttu-id="87a41-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87a41-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```





