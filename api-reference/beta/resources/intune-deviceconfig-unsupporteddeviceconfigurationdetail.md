---
title: tipo de recurso unsupportedDeviceConfigurationDetail
description: Uma descrição do motivo pelo qual uma entidade não é suportada.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f033e30400e3c198f325507030b2267425ce8f80
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703794"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="52250-103">tipo de recurso unsupportedDeviceConfigurationDetail</span><span class="sxs-lookup"><span data-stu-id="52250-103">unsupportedDeviceConfigurationDetail resource type</span></span>

<span data-ttu-id="52250-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52250-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52250-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52250-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52250-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52250-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52250-107">Uma descrição do motivo pelo qual uma entidade não é suportada.</span><span class="sxs-lookup"><span data-stu-id="52250-107">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="52250-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52250-108">Properties</span></span>
|<span data-ttu-id="52250-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52250-109">Property</span></span>|<span data-ttu-id="52250-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="52250-110">Type</span></span>|<span data-ttu-id="52250-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="52250-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52250-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="52250-112">message</span></span>|<span data-ttu-id="52250-113">String</span><span class="sxs-lookup"><span data-stu-id="52250-113">String</span></span>|<span data-ttu-id="52250-114">Uma mensagem explicando por que uma entidade não é suportada.</span><span class="sxs-lookup"><span data-stu-id="52250-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="52250-115">propertyName</span><span class="sxs-lookup"><span data-stu-id="52250-115">propertyName</span></span>|<span data-ttu-id="52250-116">String</span><span class="sxs-lookup"><span data-stu-id="52250-116">String</span></span>|<span data-ttu-id="52250-117">Se a mensagem estiver relacionada a uma propriedade específica na entidade original, o nome dessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="52250-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52250-118">Relações</span><span class="sxs-lookup"><span data-stu-id="52250-118">Relationships</span></span>
<span data-ttu-id="52250-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52250-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52250-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52250-120">JSON Representation</span></span>
<span data-ttu-id="52250-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52250-121">Here is a JSON representation of the resource.</span></span>
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





