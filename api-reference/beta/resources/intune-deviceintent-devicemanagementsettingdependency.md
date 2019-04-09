---
title: tipo de recurso deviceManagementSettingDependency
description: Informações de dependência de uma configuração
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 31de8057be462c7c8a5ef6c6becd0c1a769a96b0
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522353"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="0656b-103">tipo de recurso deviceManagementSettingDependency</span><span class="sxs-lookup"><span data-stu-id="0656b-103">deviceManagementSettingDependency resource type</span></span>

> <span data-ttu-id="0656b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0656b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0656b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0656b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0656b-106">Informações de dependência de uma configuração</span><span class="sxs-lookup"><span data-stu-id="0656b-106">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="0656b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0656b-107">Properties</span></span>
|<span data-ttu-id="0656b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0656b-108">Property</span></span>|<span data-ttu-id="0656b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0656b-109">Type</span></span>|<span data-ttu-id="0656b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0656b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0656b-111">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="0656b-111">definitionId</span></span>|<span data-ttu-id="0656b-112">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0656b-112">String</span></span>|<span data-ttu-id="0656b-113">A ID da definição de configuração da configuração dependente</span><span class="sxs-lookup"><span data-stu-id="0656b-113">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="0656b-114">as</span><span class="sxs-lookup"><span data-stu-id="0656b-114">constraints</span></span>|<span data-ttu-id="0656b-115">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="0656b-115">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="0656b-116">Conjunto de restrições para o valor da configuração de dependência</span><span class="sxs-lookup"><span data-stu-id="0656b-116">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="0656b-117">Relações</span><span class="sxs-lookup"><span data-stu-id="0656b-117">Relationships</span></span>
<span data-ttu-id="0656b-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0656b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0656b-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0656b-119">JSON Representation</span></span>
<span data-ttu-id="0656b-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0656b-120">Here is a JSON representation of the resource.</span></span>
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







