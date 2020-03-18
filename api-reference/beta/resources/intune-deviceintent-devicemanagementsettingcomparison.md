---
title: tipo de recurso deviceManagementSettingComparison
description: Entidade que representa o resultado da comparação da configuração
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5a91dc3ce4cb7e8730f346800d53740db78e5526
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785348"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a><span data-ttu-id="cf462-103">tipo de recurso deviceManagementSettingComparison</span><span class="sxs-lookup"><span data-stu-id="cf462-103">deviceManagementSettingComparison resource type</span></span>

> <span data-ttu-id="cf462-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf462-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf462-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf462-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf462-106">Entidade que representa o resultado da comparação da configuração</span><span class="sxs-lookup"><span data-stu-id="cf462-106">Entity representing setting comparison result</span></span>

## <a name="properties"></a><span data-ttu-id="cf462-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf462-107">Properties</span></span>
|<span data-ttu-id="cf462-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf462-108">Property</span></span>|<span data-ttu-id="cf462-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf462-109">Type</span></span>|<span data-ttu-id="cf462-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf462-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf462-111">id</span><span class="sxs-lookup"><span data-stu-id="cf462-111">id</span></span>|<span data-ttu-id="cf462-112">String</span><span class="sxs-lookup"><span data-stu-id="cf462-112">String</span></span>|<span data-ttu-id="cf462-113">A ID da configuração</span><span class="sxs-lookup"><span data-stu-id="cf462-113">The setting ID</span></span>|
|<span data-ttu-id="cf462-114">displayName</span><span class="sxs-lookup"><span data-stu-id="cf462-114">displayName</span></span>|<span data-ttu-id="cf462-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf462-115">String</span></span>|<span data-ttu-id="cf462-116">O nome de exibição da configuração</span><span class="sxs-lookup"><span data-stu-id="cf462-116">The setting's display name</span></span>|
|<span data-ttu-id="cf462-117">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="cf462-117">definitionId</span></span>|<span data-ttu-id="cf462-118">String</span><span class="sxs-lookup"><span data-stu-id="cf462-118">String</span></span>|<span data-ttu-id="cf462-119">A ID da definição de configuração dessa instância</span><span class="sxs-lookup"><span data-stu-id="cf462-119">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="cf462-120">currentValueJson</span><span class="sxs-lookup"><span data-stu-id="cf462-120">currentValueJson</span></span>|<span data-ttu-id="cf462-121">String</span><span class="sxs-lookup"><span data-stu-id="cf462-121">String</span></span>|<span data-ttu-id="cf462-122">Representação JSON do valor da configuração de modelo de intenção atual (ou)</span><span class="sxs-lookup"><span data-stu-id="cf462-122">JSON representation of current intent (or) template setting's value</span></span>|
|<span data-ttu-id="cf462-123">newValueJson</span><span class="sxs-lookup"><span data-stu-id="cf462-123">newValueJson</span></span>|<span data-ttu-id="cf462-124">String</span><span class="sxs-lookup"><span data-stu-id="cf462-124">String</span></span>|<span data-ttu-id="cf462-125">Representação JSON do valor da configuração de um novo modelo</span><span class="sxs-lookup"><span data-stu-id="cf462-125">JSON representation of new template setting's value</span></span>|
|<span data-ttu-id="cf462-126">comparisonResult</span><span class="sxs-lookup"><span data-stu-id="cf462-126">comparisonResult</span></span>|[<span data-ttu-id="cf462-127">deviceManagementComparisonResult</span><span class="sxs-lookup"><span data-stu-id="cf462-127">deviceManagementComparisonResult</span></span>](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|<span data-ttu-id="cf462-128">Configurando o resultado da comparação.</span><span class="sxs-lookup"><span data-stu-id="cf462-128">Setting comparison result.</span></span> <span data-ttu-id="cf462-129">Os valores possíveis são: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span><span class="sxs-lookup"><span data-stu-id="cf462-129">Possible values are: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf462-130">Relações</span><span class="sxs-lookup"><span data-stu-id="cf462-130">Relationships</span></span>
<span data-ttu-id="cf462-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cf462-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf462-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf462-132">JSON Representation</span></span>
<span data-ttu-id="cf462-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf462-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingComparison"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingComparison",
  "id": "String (identifier)",
  "displayName": "String",
  "definitionId": "String",
  "currentValueJson": "String",
  "newValueJson": "String",
  "comparisonResult": "String"
}
```



