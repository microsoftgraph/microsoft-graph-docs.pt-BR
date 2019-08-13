---
title: tipo de recurso deviceManagementSettingComparison
description: Entidade que representa o resultado da comparação da configuração
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6e8c886e3464070d0dba8779741ed65681a764de
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364737"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a><span data-ttu-id="79598-103">tipo de recurso deviceManagementSettingComparison</span><span class="sxs-lookup"><span data-stu-id="79598-103">deviceManagementSettingComparison resource type</span></span>

> <span data-ttu-id="79598-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79598-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79598-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79598-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79598-106">Entidade que representa o resultado da comparação da configuração</span><span class="sxs-lookup"><span data-stu-id="79598-106">Entity representing setting comparison result</span></span>

## <a name="properties"></a><span data-ttu-id="79598-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79598-107">Properties</span></span>
|<span data-ttu-id="79598-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79598-108">Property</span></span>|<span data-ttu-id="79598-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="79598-109">Type</span></span>|<span data-ttu-id="79598-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="79598-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79598-111">id</span><span class="sxs-lookup"><span data-stu-id="79598-111">id</span></span>|<span data-ttu-id="79598-112">String</span><span class="sxs-lookup"><span data-stu-id="79598-112">String</span></span>|<span data-ttu-id="79598-113">A ID da configuração</span><span class="sxs-lookup"><span data-stu-id="79598-113">The setting ID</span></span>|
|<span data-ttu-id="79598-114">displayName</span><span class="sxs-lookup"><span data-stu-id="79598-114">displayName</span></span>|<span data-ttu-id="79598-115">String</span><span class="sxs-lookup"><span data-stu-id="79598-115">String</span></span>|<span data-ttu-id="79598-116">O nome de exibição da configuração</span><span class="sxs-lookup"><span data-stu-id="79598-116">The setting's display name</span></span>|
|<span data-ttu-id="79598-117">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="79598-117">definitionId</span></span>|<span data-ttu-id="79598-118">String</span><span class="sxs-lookup"><span data-stu-id="79598-118">String</span></span>|<span data-ttu-id="79598-119">A ID da definição de configuração dessa instância</span><span class="sxs-lookup"><span data-stu-id="79598-119">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="79598-120">currentValueJson</span><span class="sxs-lookup"><span data-stu-id="79598-120">currentValueJson</span></span>|<span data-ttu-id="79598-121">String</span><span class="sxs-lookup"><span data-stu-id="79598-121">String</span></span>|<span data-ttu-id="79598-122">Representação JSON do valor da configuração de modelo de intenção atual (ou)</span><span class="sxs-lookup"><span data-stu-id="79598-122">JSON representation of current intent (or) template setting's value</span></span>|
|<span data-ttu-id="79598-123">newValueJson</span><span class="sxs-lookup"><span data-stu-id="79598-123">newValueJson</span></span>|<span data-ttu-id="79598-124">String</span><span class="sxs-lookup"><span data-stu-id="79598-124">String</span></span>|<span data-ttu-id="79598-125">Representação JSON do valor da configuração de um novo modelo</span><span class="sxs-lookup"><span data-stu-id="79598-125">JSON representation of new template setting's value</span></span>|
|<span data-ttu-id="79598-126">comparisonResult</span><span class="sxs-lookup"><span data-stu-id="79598-126">comparisonResult</span></span>|[<span data-ttu-id="79598-127">deviceManagementComparisonResult</span><span class="sxs-lookup"><span data-stu-id="79598-127">deviceManagementComparisonResult</span></span>](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|<span data-ttu-id="79598-128">Configurando o resultado da comparação.</span><span class="sxs-lookup"><span data-stu-id="79598-128">Setting comparison result.</span></span> <span data-ttu-id="79598-129">Os valores possíveis são: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span><span class="sxs-lookup"><span data-stu-id="79598-129">Possible values are: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79598-130">Relações</span><span class="sxs-lookup"><span data-stu-id="79598-130">Relationships</span></span>
<span data-ttu-id="79598-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79598-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79598-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79598-132">JSON Representation</span></span>
<span data-ttu-id="79598-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79598-133">Here is a JSON representation of the resource.</span></span>
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



