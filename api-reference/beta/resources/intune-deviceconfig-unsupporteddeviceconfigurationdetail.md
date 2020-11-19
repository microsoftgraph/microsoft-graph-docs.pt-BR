---
title: tipo de recurso unsupportedDeviceConfigurationDetail
description: Uma descrição do motivo pelo qual uma entidade não é suportada.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0d03c25d542d598aab7df9763baa33956f9a6a01
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276417"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="f50a7-103">tipo de recurso unsupportedDeviceConfigurationDetail</span><span class="sxs-lookup"><span data-stu-id="f50a7-103">unsupportedDeviceConfigurationDetail resource type</span></span>

<span data-ttu-id="f50a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f50a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f50a7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f50a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f50a7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f50a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f50a7-107">Uma descrição do motivo pelo qual uma entidade não é suportada.</span><span class="sxs-lookup"><span data-stu-id="f50a7-107">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="f50a7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f50a7-108">Properties</span></span>
|<span data-ttu-id="f50a7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f50a7-109">Property</span></span>|<span data-ttu-id="f50a7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f50a7-110">Type</span></span>|<span data-ttu-id="f50a7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f50a7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f50a7-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="f50a7-112">message</span></span>|<span data-ttu-id="f50a7-113">String</span><span class="sxs-lookup"><span data-stu-id="f50a7-113">String</span></span>|<span data-ttu-id="f50a7-114">Uma mensagem explicando por que uma entidade não é suportada.</span><span class="sxs-lookup"><span data-stu-id="f50a7-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="f50a7-115">propertyName</span><span class="sxs-lookup"><span data-stu-id="f50a7-115">propertyName</span></span>|<span data-ttu-id="f50a7-116">String</span><span class="sxs-lookup"><span data-stu-id="f50a7-116">String</span></span>|<span data-ttu-id="f50a7-117">Se a mensagem estiver relacionada a uma propriedade específica na entidade original, o nome dessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="f50a7-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f50a7-118">Relações</span><span class="sxs-lookup"><span data-stu-id="f50a7-118">Relationships</span></span>
<span data-ttu-id="f50a7-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f50a7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f50a7-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f50a7-120">JSON Representation</span></span>
<span data-ttu-id="f50a7-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f50a7-121">Here is a JSON representation of the resource.</span></span>
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




