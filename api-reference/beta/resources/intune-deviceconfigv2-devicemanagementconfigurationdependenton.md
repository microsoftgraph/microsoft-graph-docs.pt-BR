---
title: tipo de recurso deviceManagementConfigurationDependentOn
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67e4f4b542fa5d295a7abcd92665325b49349069
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241179"
---
# <a name="devicemanagementconfigurationdependenton-resource-type"></a><span data-ttu-id="f3ed0-103">tipo de recurso deviceManagementConfigurationDependentOn</span><span class="sxs-lookup"><span data-stu-id="f3ed0-103">deviceManagementConfigurationDependentOn resource type</span></span>

<span data-ttu-id="f3ed0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3ed0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3ed0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3ed0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3ed0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3ed0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3ed0-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f3ed0-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f3ed0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3ed0-108">Properties</span></span>
|<span data-ttu-id="f3ed0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3ed0-109">Property</span></span>|<span data-ttu-id="f3ed0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3ed0-110">Type</span></span>|<span data-ttu-id="f3ed0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3ed0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3ed0-112">dependente</span><span class="sxs-lookup"><span data-stu-id="f3ed0-112">dependentOn</span></span>|<span data-ttu-id="f3ed0-113">String</span><span class="sxs-lookup"><span data-stu-id="f3ed0-113">String</span></span>|<span data-ttu-id="f3ed0-114">Identificador de configuração pai/opção de configuração pai dependente</span><span class="sxs-lookup"><span data-stu-id="f3ed0-114">Identifier of parent setting/ parent setting option dependent on</span></span>|
|<span data-ttu-id="f3ed0-115">parentSettingId</span><span class="sxs-lookup"><span data-stu-id="f3ed0-115">parentSettingId</span></span>|<span data-ttu-id="f3ed0-116">String</span><span class="sxs-lookup"><span data-stu-id="f3ed0-116">String</span></span>|<span data-ttu-id="f3ed0-117">Identificador da configuração pai/ID de configuração pai dependente</span><span class="sxs-lookup"><span data-stu-id="f3ed0-117">Identifier of parent setting/ parent setting id dependent on</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3ed0-118">Relações</span><span class="sxs-lookup"><span data-stu-id="f3ed0-118">Relationships</span></span>
<span data-ttu-id="f3ed0-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f3ed0-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3ed0-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3ed0-120">JSON Representation</span></span>
<span data-ttu-id="f3ed0-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3ed0-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationDependentOn",
  "dependentOn": "String",
  "parentSettingId": "String"
}
```




