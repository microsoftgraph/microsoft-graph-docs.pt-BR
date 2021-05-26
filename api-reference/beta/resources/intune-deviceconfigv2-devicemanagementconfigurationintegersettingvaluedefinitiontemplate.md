---
title: Tipo de recurso deviceManagementConfigurationIntegerSettingValueDefinitionTemplate
description: Modelo de definição de valor de configuração de inteiro
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 488c71fd7f242604a2bcd8bbdcc2ca7f526bd4d7
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666781"
---
# <a name="devicemanagementconfigurationintegersettingvaluedefinitiontemplate-resource-type"></a><span data-ttu-id="9b2ec-103">Tipo de recurso deviceManagementConfigurationIntegerSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="9b2ec-103">deviceManagementConfigurationIntegerSettingValueDefinitionTemplate resource type</span></span>

<span data-ttu-id="9b2ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b2ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b2ec-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b2ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b2ec-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b2ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b2ec-107">Modelo de definição de valor de configuração de inteiro</span><span class="sxs-lookup"><span data-stu-id="9b2ec-107">Integer Setting Value Definition Template</span></span>

## <a name="properties"></a><span data-ttu-id="9b2ec-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b2ec-108">Properties</span></span>
|<span data-ttu-id="9b2ec-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b2ec-109">Property</span></span>|<span data-ttu-id="9b2ec-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b2ec-110">Type</span></span>|<span data-ttu-id="9b2ec-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b2ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b2ec-112">minValue</span><span class="sxs-lookup"><span data-stu-id="9b2ec-112">minValue</span></span>|<span data-ttu-id="9b2ec-113">Int32</span><span class="sxs-lookup"><span data-stu-id="9b2ec-113">Int32</span></span>|<span data-ttu-id="9b2ec-114">Valor mínimo de configuração de inteiro.</span><span class="sxs-lookup"><span data-stu-id="9b2ec-114">Integer Setting Minimum Value.</span></span> <span data-ttu-id="9b2ec-115">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="9b2ec-115">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="9b2ec-116">maxValue</span><span class="sxs-lookup"><span data-stu-id="9b2ec-116">maxValue</span></span>|<span data-ttu-id="9b2ec-117">Int32</span><span class="sxs-lookup"><span data-stu-id="9b2ec-117">Int32</span></span>|<span data-ttu-id="9b2ec-118">Valor máximo de configuração de inteiro.</span><span class="sxs-lookup"><span data-stu-id="9b2ec-118">Integer Setting Maximum Value.</span></span> <span data-ttu-id="9b2ec-119">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="9b2ec-119">Valid values -2147483648 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b2ec-120">Relações</span><span class="sxs-lookup"><span data-stu-id="9b2ec-120">Relationships</span></span>
<span data-ttu-id="9b2ec-121">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9b2ec-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b2ec-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b2ec-122">JSON Representation</span></span>
<span data-ttu-id="9b2ec-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b2ec-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate",
  "minValue": 1024,
  "maxValue": 1024
}
```




