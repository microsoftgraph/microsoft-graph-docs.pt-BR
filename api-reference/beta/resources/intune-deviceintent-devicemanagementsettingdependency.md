---
title: tipo de recurso deviceManagementSettingDependency
description: Informações de dependência de uma configuração
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8f75e4590336f94520c1dc43b437a36048a230c
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636732"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="0b6b1-103">tipo de recurso deviceManagementSettingDependency</span><span class="sxs-lookup"><span data-stu-id="0b6b1-103">deviceManagementSettingDependency resource type</span></span>

> <span data-ttu-id="0b6b1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0b6b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b6b1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b6b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b6b1-106">Informações de dependência de uma configuração</span><span class="sxs-lookup"><span data-stu-id="0b6b1-106">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="0b6b1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b6b1-107">Properties</span></span>
|<span data-ttu-id="0b6b1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b6b1-108">Property</span></span>|<span data-ttu-id="0b6b1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b6b1-109">Type</span></span>|<span data-ttu-id="0b6b1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b6b1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b6b1-111">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="0b6b1-111">definitionId</span></span>|<span data-ttu-id="0b6b1-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b6b1-112">String</span></span>|<span data-ttu-id="0b6b1-113">A ID da definição de configuração da configuração dependente</span><span class="sxs-lookup"><span data-stu-id="0b6b1-113">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="0b6b1-114">as</span><span class="sxs-lookup"><span data-stu-id="0b6b1-114">constraints</span></span>|<span data-ttu-id="0b6b1-115">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="0b6b1-115">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="0b6b1-116">Conjunto de restrições para o valor da configuração de dependência</span><span class="sxs-lookup"><span data-stu-id="0b6b1-116">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b6b1-117">Relações</span><span class="sxs-lookup"><span data-stu-id="0b6b1-117">Relationships</span></span>
<span data-ttu-id="0b6b1-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b6b1-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b6b1-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b6b1-119">JSON Representation</span></span>
<span data-ttu-id="0b6b1-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b6b1-120">Here is a JSON representation of the resource.</span></span>
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



