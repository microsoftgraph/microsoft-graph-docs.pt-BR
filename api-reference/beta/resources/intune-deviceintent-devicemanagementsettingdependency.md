---
title: tipo de recurso deviceManagementSettingDependency
description: Informações de dependência de uma configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b96555b98f23206d9c85bb40cf567ed0938da5d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061200"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="e971b-103">tipo de recurso deviceManagementSettingDependency</span><span class="sxs-lookup"><span data-stu-id="e971b-103">deviceManagementSettingDependency resource type</span></span>

<span data-ttu-id="e971b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e971b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e971b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e971b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e971b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e971b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e971b-107">Informações de dependência de uma configuração</span><span class="sxs-lookup"><span data-stu-id="e971b-107">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="e971b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e971b-108">Properties</span></span>
|<span data-ttu-id="e971b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e971b-109">Property</span></span>|<span data-ttu-id="e971b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e971b-110">Type</span></span>|<span data-ttu-id="e971b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e971b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e971b-112">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="e971b-112">definitionId</span></span>|<span data-ttu-id="e971b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e971b-113">String</span></span>|<span data-ttu-id="e971b-114">A ID da definição de configuração da configuração dependente</span><span class="sxs-lookup"><span data-stu-id="e971b-114">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="e971b-115">as</span><span class="sxs-lookup"><span data-stu-id="e971b-115">constraints</span></span>|<span data-ttu-id="e971b-116">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="e971b-116">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="e971b-117">Conjunto de restrições para o valor da configuração de dependência</span><span class="sxs-lookup"><span data-stu-id="e971b-117">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="e971b-118">Relações</span><span class="sxs-lookup"><span data-stu-id="e971b-118">Relationships</span></span>
<span data-ttu-id="e971b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e971b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e971b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e971b-120">JSON Representation</span></span>
<span data-ttu-id="e971b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e971b-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDependency",
  "definitionId": "String",
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "String"
      ]
    }
  ]
}
```






