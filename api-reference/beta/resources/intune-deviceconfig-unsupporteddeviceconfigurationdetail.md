---
title: tipo de recurso unsupportedDeviceConfigurationDetail
description: Uma descrição do motivo pelo qual uma entidade não é suportada.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 53ca6773c3b5341c3f0aae07369b4af80643728d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969601"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="6bc53-103">tipo de recurso unsupportedDeviceConfigurationDetail</span><span class="sxs-lookup"><span data-stu-id="6bc53-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="6bc53-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6bc53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bc53-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6bc53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bc53-106">Uma descrição do motivo pelo qual uma entidade não é suportada.</span><span class="sxs-lookup"><span data-stu-id="6bc53-106">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="6bc53-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6bc53-107">Properties</span></span>
|<span data-ttu-id="6bc53-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6bc53-108">Property</span></span>|<span data-ttu-id="6bc53-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bc53-109">Type</span></span>|<span data-ttu-id="6bc53-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bc53-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bc53-111">mensagem</span><span class="sxs-lookup"><span data-stu-id="6bc53-111">message</span></span>|<span data-ttu-id="6bc53-112">String</span><span class="sxs-lookup"><span data-stu-id="6bc53-112">String</span></span>|<span data-ttu-id="6bc53-113">Uma mensagem explicando por que uma entidade não é suportada.</span><span class="sxs-lookup"><span data-stu-id="6bc53-113">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="6bc53-114">NomeDaPropriedade</span><span class="sxs-lookup"><span data-stu-id="6bc53-114">propertyName</span></span>|<span data-ttu-id="6bc53-115">String</span><span class="sxs-lookup"><span data-stu-id="6bc53-115">String</span></span>|<span data-ttu-id="6bc53-116">Se a mensagem estiver relacionada a uma propriedade específica na entidade original, o nome dessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="6bc53-116">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bc53-117">Relações</span><span class="sxs-lookup"><span data-stu-id="6bc53-117">Relationships</span></span>
<span data-ttu-id="6bc53-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6bc53-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6bc53-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6bc53-119">JSON Representation</span></span>
<span data-ttu-id="6bc53-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6bc53-120">Here is a JSON representation of the resource.</span></span>
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





