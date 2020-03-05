---
title: tipo de recurso deviceManagementSettingDependency
description: Informações de dependência de uma configuração
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9cb6abb17963a9c22e027a4ba56eadfd3b07f6a8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525254"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="41272-103">tipo de recurso deviceManagementSettingDependency</span><span class="sxs-lookup"><span data-stu-id="41272-103">deviceManagementSettingDependency resource type</span></span>

<span data-ttu-id="41272-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="41272-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41272-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="41272-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41272-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41272-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41272-107">Informações de dependência de uma configuração</span><span class="sxs-lookup"><span data-stu-id="41272-107">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="41272-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41272-108">Properties</span></span>
|<span data-ttu-id="41272-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41272-109">Property</span></span>|<span data-ttu-id="41272-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="41272-110">Type</span></span>|<span data-ttu-id="41272-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="41272-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41272-112">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="41272-112">definitionId</span></span>|<span data-ttu-id="41272-113">String</span><span class="sxs-lookup"><span data-stu-id="41272-113">String</span></span>|<span data-ttu-id="41272-114">A ID da definição de configuração da configuração dependente</span><span class="sxs-lookup"><span data-stu-id="41272-114">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="41272-115">as</span><span class="sxs-lookup"><span data-stu-id="41272-115">constraints</span></span>|<span data-ttu-id="41272-116">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="41272-116">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="41272-117">Conjunto de restrições para o valor da configuração de dependência</span><span class="sxs-lookup"><span data-stu-id="41272-117">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="41272-118">Relações</span><span class="sxs-lookup"><span data-stu-id="41272-118">Relationships</span></span>
<span data-ttu-id="41272-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41272-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41272-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41272-120">JSON Representation</span></span>
<span data-ttu-id="41272-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41272-121">Here is a JSON representation of the resource.</span></span>
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



