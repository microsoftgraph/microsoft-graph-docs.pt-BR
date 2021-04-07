---
title: Tipo de recurso chromeOSDeviceProperty
description: Representa uma propriedade do dispositivo ChromeOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 42b4903965d90641955659277360c46428562ed4
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612106"
---
# <a name="chromeosdeviceproperty-resource-type"></a><span data-ttu-id="09312-103">Tipo de recurso chromeOSDeviceProperty</span><span class="sxs-lookup"><span data-stu-id="09312-103">chromeOSDeviceProperty resource type</span></span>

<span data-ttu-id="09312-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09312-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09312-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09312-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09312-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09312-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09312-107">Representa uma propriedade do dispositivo ChromeOS.</span><span class="sxs-lookup"><span data-stu-id="09312-107">Represents a property of the ChromeOS device.</span></span>

## <a name="properties"></a><span data-ttu-id="09312-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09312-108">Properties</span></span>
|<span data-ttu-id="09312-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09312-109">Property</span></span>|<span data-ttu-id="09312-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="09312-110">Type</span></span>|<span data-ttu-id="09312-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="09312-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09312-112">nome</span><span class="sxs-lookup"><span data-stu-id="09312-112">name</span></span>|<span data-ttu-id="09312-113">String</span><span class="sxs-lookup"><span data-stu-id="09312-113">String</span></span>|<span data-ttu-id="09312-114">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="09312-114">Name of the property</span></span>|
|<span data-ttu-id="09312-115">value</span><span class="sxs-lookup"><span data-stu-id="09312-115">value</span></span>|<span data-ttu-id="09312-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09312-116">String</span></span>|<span data-ttu-id="09312-117">Valor da propriedade</span><span class="sxs-lookup"><span data-stu-id="09312-117">Value of the property</span></span>|
|<span data-ttu-id="09312-118">valueType</span><span class="sxs-lookup"><span data-stu-id="09312-118">valueType</span></span>|<span data-ttu-id="09312-119">String</span><span class="sxs-lookup"><span data-stu-id="09312-119">String</span></span>|<span data-ttu-id="09312-120">Tipo do valor</span><span class="sxs-lookup"><span data-stu-id="09312-120">Type of the value</span></span>|
|<span data-ttu-id="09312-121">atualizável</span><span class="sxs-lookup"><span data-stu-id="09312-121">updatable</span></span>|<span data-ttu-id="09312-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="09312-122">Boolean</span></span>|<span data-ttu-id="09312-123">Se essa propriedade é atualizável</span><span class="sxs-lookup"><span data-stu-id="09312-123">Whether this property is updatable</span></span>|

## <a name="relationships"></a><span data-ttu-id="09312-124">Relações</span><span class="sxs-lookup"><span data-stu-id="09312-124">Relationships</span></span>
<span data-ttu-id="09312-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="09312-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09312-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09312-126">JSON Representation</span></span>
<span data-ttu-id="09312-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09312-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chromeOSDeviceProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chromeOSDeviceProperty",
  "name": "String",
  "value": "String",
  "valueType": "String",
  "updatable": true
}
```




