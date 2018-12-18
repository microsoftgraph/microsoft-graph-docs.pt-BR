---
title: tipo de recurso de unsupportedDeviceConfigurationDetail
description: Uma descrição por que não há suporte para uma entidade.
author: tfitzmac
ms.openlocfilehash: 4cccf49366a803e5f964605a4dc4ba7f56707823
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344048"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="96acf-103">tipo de recurso de unsupportedDeviceConfigurationDetail</span><span class="sxs-lookup"><span data-stu-id="96acf-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="96acf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="96acf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96acf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="96acf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96acf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="96acf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96acf-107">Uma descrição por que não há suporte para uma entidade.</span><span class="sxs-lookup"><span data-stu-id="96acf-107">A description of why an entity is unsupported.</span></span>
## <a name="properties"></a><span data-ttu-id="96acf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96acf-108">Properties</span></span>
|<span data-ttu-id="96acf-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96acf-109">Property</span></span>|<span data-ttu-id="96acf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="96acf-110">Type</span></span>|<span data-ttu-id="96acf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="96acf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96acf-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="96acf-112">message</span></span>|<span data-ttu-id="96acf-113">String</span><span class="sxs-lookup"><span data-stu-id="96acf-113">String</span></span>|<span data-ttu-id="96acf-114">Uma mensagem que explica por que não há suporte para uma entidade.</span><span class="sxs-lookup"><span data-stu-id="96acf-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="96acf-115">propertyName</span><span class="sxs-lookup"><span data-stu-id="96acf-115">propertyName</span></span>|<span data-ttu-id="96acf-116">String</span><span class="sxs-lookup"><span data-stu-id="96acf-116">String</span></span>|<span data-ttu-id="96acf-117">Se a mensagem está relacionada a uma propriedade específica à entidade original e, em seguida, o nome dessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="96acf-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96acf-118">Relações</span><span class="sxs-lookup"><span data-stu-id="96acf-118">Relationships</span></span>
<span data-ttu-id="96acf-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96acf-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="96acf-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96acf-120">JSON Representation</span></span>
<span data-ttu-id="96acf-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96acf-121">Here is a JSON representation of the resource.</span></span>
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





