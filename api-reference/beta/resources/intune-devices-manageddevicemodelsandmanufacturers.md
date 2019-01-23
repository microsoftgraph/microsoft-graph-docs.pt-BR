---
title: tipo de recurso de managedDeviceModelsAndManufacturers
description: Modelos e fabricantes meatadata para dispositivos gerenciados na conta
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: afcf64cb0e8db4e24ce061490ecc593595690930
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396788"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="94dfd-103">tipo de recurso de managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="94dfd-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="94dfd-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="94dfd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="94dfd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="94dfd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94dfd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="94dfd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94dfd-107">Modelos e fabricantes meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="94dfd-107">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="94dfd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94dfd-108">Properties</span></span>
|<span data-ttu-id="94dfd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94dfd-109">Property</span></span>|<span data-ttu-id="94dfd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="94dfd-110">Type</span></span>|<span data-ttu-id="94dfd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="94dfd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94dfd-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="94dfd-112">deviceModels</span></span>|<span data-ttu-id="94dfd-113">String collection</span><span class="sxs-lookup"><span data-stu-id="94dfd-113">String collection</span></span>|<span data-ttu-id="94dfd-114">Lista de modelos para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="94dfd-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="94dfd-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="94dfd-115">deviceManufacturers</span></span>|<span data-ttu-id="94dfd-116">String collection</span><span class="sxs-lookup"><span data-stu-id="94dfd-116">String collection</span></span>|<span data-ttu-id="94dfd-117">Lista de fabricantes de dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="94dfd-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="94dfd-118">Relações</span><span class="sxs-lookup"><span data-stu-id="94dfd-118">Relationships</span></span>
<span data-ttu-id="94dfd-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94dfd-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94dfd-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94dfd-120">JSON Representation</span></span>
<span data-ttu-id="94dfd-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94dfd-121">Here is a JSON representation of the resource.</span></span>
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




