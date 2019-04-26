---
title: tipo de recurso deviceManagementSettingDependency
description: Informações de dependência de uma configuração
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b506ff636cf2a44b466d531f60924cd7eaa2c7b3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550704"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="8e3f6-103">tipo de recurso deviceManagementSettingDependency</span><span class="sxs-lookup"><span data-stu-id="8e3f6-103">deviceManagementSettingDependency resource type</span></span>

> <span data-ttu-id="8e3f6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e3f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e3f6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e3f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e3f6-106">Informações de dependência de uma configuração</span><span class="sxs-lookup"><span data-stu-id="8e3f6-106">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="8e3f6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e3f6-107">Properties</span></span>
|<span data-ttu-id="8e3f6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e3f6-108">Property</span></span>|<span data-ttu-id="8e3f6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e3f6-109">Type</span></span>|<span data-ttu-id="8e3f6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e3f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e3f6-111">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="8e3f6-111">definitionId</span></span>|<span data-ttu-id="8e3f6-112">String</span><span class="sxs-lookup"><span data-stu-id="8e3f6-112">String</span></span>|<span data-ttu-id="8e3f6-113">A ID da definição de configuração da configuração dependente</span><span class="sxs-lookup"><span data-stu-id="8e3f6-113">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="8e3f6-114">as</span><span class="sxs-lookup"><span data-stu-id="8e3f6-114">constraints</span></span>|<span data-ttu-id="8e3f6-115">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="8e3f6-115">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="8e3f6-116">Conjunto de restrições para o valor da configuração de dependência</span><span class="sxs-lookup"><span data-stu-id="8e3f6-116">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e3f6-117">Relações</span><span class="sxs-lookup"><span data-stu-id="8e3f6-117">Relationships</span></span>
<span data-ttu-id="8e3f6-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e3f6-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e3f6-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e3f6-119">JSON Representation</span></span>
<span data-ttu-id="8e3f6-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e3f6-120">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ]
}
```





