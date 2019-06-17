---
title: tipo de recurso unsupportedDeviceConfigurationDetail
description: Uma descrição do motivo pelo qual uma entidade não é suportada.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce838f73c4ad02ecb29d540a9f0d4af065796993
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978966"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="836bf-103">tipo de recurso unsupportedDeviceConfigurationDetail</span><span class="sxs-lookup"><span data-stu-id="836bf-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="836bf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="836bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="836bf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="836bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="836bf-106">Uma descrição do motivo pelo qual uma entidade não é suportada.</span><span class="sxs-lookup"><span data-stu-id="836bf-106">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="836bf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="836bf-107">Properties</span></span>
|<span data-ttu-id="836bf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="836bf-108">Property</span></span>|<span data-ttu-id="836bf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="836bf-109">Type</span></span>|<span data-ttu-id="836bf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="836bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="836bf-111">mensagem</span><span class="sxs-lookup"><span data-stu-id="836bf-111">message</span></span>|<span data-ttu-id="836bf-112">String</span><span class="sxs-lookup"><span data-stu-id="836bf-112">String</span></span>|<span data-ttu-id="836bf-113">Uma mensagem explicando por que uma entidade não é suportada.</span><span class="sxs-lookup"><span data-stu-id="836bf-113">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="836bf-114">NomeDaPropriedade</span><span class="sxs-lookup"><span data-stu-id="836bf-114">propertyName</span></span>|<span data-ttu-id="836bf-115">String</span><span class="sxs-lookup"><span data-stu-id="836bf-115">String</span></span>|<span data-ttu-id="836bf-116">Se a mensagem estiver relacionada a uma propriedade específica na entidade original, o nome dessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="836bf-116">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="836bf-117">Relações</span><span class="sxs-lookup"><span data-stu-id="836bf-117">Relationships</span></span>
<span data-ttu-id="836bf-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="836bf-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="836bf-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="836bf-119">JSON Representation</span></span>
<span data-ttu-id="836bf-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="836bf-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```





