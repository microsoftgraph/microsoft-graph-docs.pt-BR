---
title: tipo de recurso deviceManagementSettingComparison
description: Entidade que representa o resultado da comparação da configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0463da79c2cedc78c5546fa86b5891468f7a4c11
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728276"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a><span data-ttu-id="6da5c-103">tipo de recurso deviceManagementSettingComparison</span><span class="sxs-lookup"><span data-stu-id="6da5c-103">deviceManagementSettingComparison resource type</span></span>

<span data-ttu-id="6da5c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6da5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6da5c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6da5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6da5c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6da5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6da5c-107">Entidade que representa o resultado da comparação da configuração</span><span class="sxs-lookup"><span data-stu-id="6da5c-107">Entity representing setting comparison result</span></span>

## <a name="properties"></a><span data-ttu-id="6da5c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6da5c-108">Properties</span></span>
|<span data-ttu-id="6da5c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6da5c-109">Property</span></span>|<span data-ttu-id="6da5c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6da5c-110">Type</span></span>|<span data-ttu-id="6da5c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6da5c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6da5c-112">id</span><span class="sxs-lookup"><span data-stu-id="6da5c-112">id</span></span>|<span data-ttu-id="6da5c-113">String</span><span class="sxs-lookup"><span data-stu-id="6da5c-113">String</span></span>|<span data-ttu-id="6da5c-114">A ID da configuração</span><span class="sxs-lookup"><span data-stu-id="6da5c-114">The setting ID</span></span>|
|<span data-ttu-id="6da5c-115">displayName</span><span class="sxs-lookup"><span data-stu-id="6da5c-115">displayName</span></span>|<span data-ttu-id="6da5c-116">String</span><span class="sxs-lookup"><span data-stu-id="6da5c-116">String</span></span>|<span data-ttu-id="6da5c-117">O nome de exibição da configuração</span><span class="sxs-lookup"><span data-stu-id="6da5c-117">The setting's display name</span></span>|
|<span data-ttu-id="6da5c-118">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="6da5c-118">definitionId</span></span>|<span data-ttu-id="6da5c-119">String</span><span class="sxs-lookup"><span data-stu-id="6da5c-119">String</span></span>|<span data-ttu-id="6da5c-120">A ID da definição de configuração dessa instância</span><span class="sxs-lookup"><span data-stu-id="6da5c-120">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="6da5c-121">currentValueJson</span><span class="sxs-lookup"><span data-stu-id="6da5c-121">currentValueJson</span></span>|<span data-ttu-id="6da5c-122">String</span><span class="sxs-lookup"><span data-stu-id="6da5c-122">String</span></span>|<span data-ttu-id="6da5c-123">Representação JSON do valor da configuração de modelo de intenção atual (ou)</span><span class="sxs-lookup"><span data-stu-id="6da5c-123">JSON representation of current intent (or) template setting's value</span></span>|
|<span data-ttu-id="6da5c-124">newValueJson</span><span class="sxs-lookup"><span data-stu-id="6da5c-124">newValueJson</span></span>|<span data-ttu-id="6da5c-125">String</span><span class="sxs-lookup"><span data-stu-id="6da5c-125">String</span></span>|<span data-ttu-id="6da5c-126">Representação JSON do valor da configuração de um novo modelo</span><span class="sxs-lookup"><span data-stu-id="6da5c-126">JSON representation of new template setting's value</span></span>|
|<span data-ttu-id="6da5c-127">comparisonResult</span><span class="sxs-lookup"><span data-stu-id="6da5c-127">comparisonResult</span></span>|[<span data-ttu-id="6da5c-128">deviceManagementComparisonResult</span><span class="sxs-lookup"><span data-stu-id="6da5c-128">deviceManagementComparisonResult</span></span>](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|<span data-ttu-id="6da5c-129">Configurando o resultado da comparação.</span><span class="sxs-lookup"><span data-stu-id="6da5c-129">Setting comparison result.</span></span> <span data-ttu-id="6da5c-130">Os valores possíveis são: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span><span class="sxs-lookup"><span data-stu-id="6da5c-130">Possible values are: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6da5c-131">Relações</span><span class="sxs-lookup"><span data-stu-id="6da5c-131">Relationships</span></span>
<span data-ttu-id="6da5c-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6da5c-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6da5c-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6da5c-133">JSON Representation</span></span>
<span data-ttu-id="6da5c-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6da5c-134">Here is a JSON representation of the resource.</span></span>
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





