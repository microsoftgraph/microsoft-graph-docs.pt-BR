---
title: tipo de recurso deviceManagementSettingDependency
description: Informações de dependência de uma configuração
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9014b3618562717c2cc9522c388034ad81213a4c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420119"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="4d662-103">tipo de recurso deviceManagementSettingDependency</span><span class="sxs-lookup"><span data-stu-id="4d662-103">deviceManagementSettingDependency resource type</span></span>

<span data-ttu-id="4d662-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d662-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d662-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4d662-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d662-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4d662-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d662-107">Informações de dependência de uma configuração</span><span class="sxs-lookup"><span data-stu-id="4d662-107">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="4d662-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d662-108">Properties</span></span>
|<span data-ttu-id="4d662-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d662-109">Property</span></span>|<span data-ttu-id="4d662-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d662-110">Type</span></span>|<span data-ttu-id="4d662-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d662-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d662-112">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="4d662-112">definitionId</span></span>|<span data-ttu-id="4d662-113">String</span><span class="sxs-lookup"><span data-stu-id="4d662-113">String</span></span>|<span data-ttu-id="4d662-114">A ID da definição de configuração da configuração dependente</span><span class="sxs-lookup"><span data-stu-id="4d662-114">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="4d662-115">as</span><span class="sxs-lookup"><span data-stu-id="4d662-115">constraints</span></span>|<span data-ttu-id="4d662-116">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="4d662-116">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="4d662-117">Conjunto de restrições para o valor da configuração de dependência</span><span class="sxs-lookup"><span data-stu-id="4d662-117">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d662-118">Relações</span><span class="sxs-lookup"><span data-stu-id="4d662-118">Relationships</span></span>
<span data-ttu-id="4d662-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4d662-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d662-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d662-120">JSON Representation</span></span>
<span data-ttu-id="4d662-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4d662-121">Here is a JSON representation of the resource.</span></span>
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



