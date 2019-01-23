---
title: tipo de recurso de unsupportedDeviceConfigurationDetail
description: Uma descrição por que não há suporte para uma entidade.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c03bdb20fc4c48fa7820e09b9212bf73250599aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400386"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="bd30d-103">tipo de recurso de unsupportedDeviceConfigurationDetail</span><span class="sxs-lookup"><span data-stu-id="bd30d-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="bd30d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="bd30d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bd30d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bd30d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd30d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="bd30d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd30d-107">Uma descrição por que não há suporte para uma entidade.</span><span class="sxs-lookup"><span data-stu-id="bd30d-107">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="bd30d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd30d-108">Properties</span></span>
|<span data-ttu-id="bd30d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd30d-109">Property</span></span>|<span data-ttu-id="bd30d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd30d-110">Type</span></span>|<span data-ttu-id="bd30d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd30d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd30d-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="bd30d-112">message</span></span>|<span data-ttu-id="bd30d-113">String</span><span class="sxs-lookup"><span data-stu-id="bd30d-113">String</span></span>|<span data-ttu-id="bd30d-114">Uma mensagem que explica por que não há suporte para uma entidade.</span><span class="sxs-lookup"><span data-stu-id="bd30d-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="bd30d-115">propertyName</span><span class="sxs-lookup"><span data-stu-id="bd30d-115">propertyName</span></span>|<span data-ttu-id="bd30d-116">String</span><span class="sxs-lookup"><span data-stu-id="bd30d-116">String</span></span>|<span data-ttu-id="bd30d-117">Se a mensagem está relacionada a uma propriedade específica à entidade original e, em seguida, o nome dessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="bd30d-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd30d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="bd30d-118">Relationships</span></span>
<span data-ttu-id="bd30d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bd30d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd30d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd30d-120">JSON Representation</span></span>
<span data-ttu-id="bd30d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bd30d-121">Here is a JSON representation of the resource.</span></span>
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




