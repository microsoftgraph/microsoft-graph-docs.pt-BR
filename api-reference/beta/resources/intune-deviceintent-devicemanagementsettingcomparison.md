---
title: tipo de recurso deviceManagementSettingComparison
description: Entidade que representa o resultado da comparação da configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e51d413dfa0e1e60fcf07e37c2806c39f62cc76
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061242"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a><span data-ttu-id="5f662-103">tipo de recurso deviceManagementSettingComparison</span><span class="sxs-lookup"><span data-stu-id="5f662-103">deviceManagementSettingComparison resource type</span></span>

<span data-ttu-id="5f662-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f662-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f662-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5f662-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f662-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f662-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f662-107">Entidade que representa o resultado da comparação da configuração</span><span class="sxs-lookup"><span data-stu-id="5f662-107">Entity representing setting comparison result</span></span>

## <a name="properties"></a><span data-ttu-id="5f662-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f662-108">Properties</span></span>
|<span data-ttu-id="5f662-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f662-109">Property</span></span>|<span data-ttu-id="5f662-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f662-110">Type</span></span>|<span data-ttu-id="5f662-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f662-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f662-112">id</span><span class="sxs-lookup"><span data-stu-id="5f662-112">id</span></span>|<span data-ttu-id="5f662-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f662-113">String</span></span>|<span data-ttu-id="5f662-114">A ID da configuração</span><span class="sxs-lookup"><span data-stu-id="5f662-114">The setting ID</span></span>|
|<span data-ttu-id="5f662-115">displayName</span><span class="sxs-lookup"><span data-stu-id="5f662-115">displayName</span></span>|<span data-ttu-id="5f662-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f662-116">String</span></span>|<span data-ttu-id="5f662-117">O nome de exibição da configuração</span><span class="sxs-lookup"><span data-stu-id="5f662-117">The setting's display name</span></span>|
|<span data-ttu-id="5f662-118">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="5f662-118">definitionId</span></span>|<span data-ttu-id="5f662-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f662-119">String</span></span>|<span data-ttu-id="5f662-120">A ID da definição de configuração dessa instância</span><span class="sxs-lookup"><span data-stu-id="5f662-120">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="5f662-121">currentValueJson</span><span class="sxs-lookup"><span data-stu-id="5f662-121">currentValueJson</span></span>|<span data-ttu-id="5f662-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f662-122">String</span></span>|<span data-ttu-id="5f662-123">Representação JSON do valor da configuração de modelo de intenção atual (ou)</span><span class="sxs-lookup"><span data-stu-id="5f662-123">JSON representation of current intent (or) template setting's value</span></span>|
|<span data-ttu-id="5f662-124">newValueJson</span><span class="sxs-lookup"><span data-stu-id="5f662-124">newValueJson</span></span>|<span data-ttu-id="5f662-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f662-125">String</span></span>|<span data-ttu-id="5f662-126">Representação JSON do valor da configuração de um novo modelo</span><span class="sxs-lookup"><span data-stu-id="5f662-126">JSON representation of new template setting's value</span></span>|
|<span data-ttu-id="5f662-127">comparisonResult</span><span class="sxs-lookup"><span data-stu-id="5f662-127">comparisonResult</span></span>|[<span data-ttu-id="5f662-128">deviceManagementComparisonResult</span><span class="sxs-lookup"><span data-stu-id="5f662-128">deviceManagementComparisonResult</span></span>](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|<span data-ttu-id="5f662-129">Configurando o resultado da comparação.</span><span class="sxs-lookup"><span data-stu-id="5f662-129">Setting comparison result.</span></span> <span data-ttu-id="5f662-130">Os valores possíveis são: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span><span class="sxs-lookup"><span data-stu-id="5f662-130">Possible values are: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f662-131">Relações</span><span class="sxs-lookup"><span data-stu-id="5f662-131">Relationships</span></span>
<span data-ttu-id="5f662-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f662-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f662-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f662-133">JSON Representation</span></span>
<span data-ttu-id="5f662-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f662-134">Here is a JSON representation of the resource.</span></span>
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






