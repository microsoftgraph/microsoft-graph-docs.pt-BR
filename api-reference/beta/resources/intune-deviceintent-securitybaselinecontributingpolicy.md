---
title: tipo de recurso securityBaselineContributingPolicy
description: O estado de conformidade da linha de base de segurança de uma configuração para um dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f62299f39d4e3670fc586a4dc07d352a992398e0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49209343"
---
# <a name="securitybaselinecontributingpolicy-resource-type"></a><span data-ttu-id="bfe13-103">tipo de recurso securityBaselineContributingPolicy</span><span class="sxs-lookup"><span data-stu-id="bfe13-103">securityBaselineContributingPolicy resource type</span></span>

<span data-ttu-id="bfe13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfe13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bfe13-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bfe13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfe13-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bfe13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfe13-107">O estado de conformidade da linha de base de segurança de uma configuração para um dispositivo</span><span class="sxs-lookup"><span data-stu-id="bfe13-107">The security baseline compliance state of a setting for a device</span></span>

## <a name="properties"></a><span data-ttu-id="bfe13-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bfe13-108">Properties</span></span>
|<span data-ttu-id="bfe13-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bfe13-109">Property</span></span>|<span data-ttu-id="bfe13-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfe13-110">Type</span></span>|<span data-ttu-id="bfe13-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfe13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfe13-112">sourceId</span><span class="sxs-lookup"><span data-stu-id="bfe13-112">sourceId</span></span>|<span data-ttu-id="bfe13-113">String</span><span class="sxs-lookup"><span data-stu-id="bfe13-113">String</span></span>|<span data-ttu-id="bfe13-114">Identificador exclusivo da política</span><span class="sxs-lookup"><span data-stu-id="bfe13-114">Unique identifier of the policy</span></span>|
|<span data-ttu-id="bfe13-115">displayName</span><span class="sxs-lookup"><span data-stu-id="bfe13-115">displayName</span></span>|<span data-ttu-id="bfe13-116">String</span><span class="sxs-lookup"><span data-stu-id="bfe13-116">String</span></span>|<span data-ttu-id="bfe13-117">Nome da política</span><span class="sxs-lookup"><span data-stu-id="bfe13-117">Name of the policy</span></span>|
|<span data-ttu-id="bfe13-118">sourceType</span><span class="sxs-lookup"><span data-stu-id="bfe13-118">sourceType</span></span>|[<span data-ttu-id="bfe13-119">securityBaselinePolicySourceType</span><span class="sxs-lookup"><span data-stu-id="bfe13-119">securityBaselinePolicySourceType</span></span>](../resources/intune-deviceintent-securitybaselinepolicysourcetype.md)|<span data-ttu-id="bfe13-120">Fonte de criação da política.</span><span class="sxs-lookup"><span data-stu-id="bfe13-120">Authoring source of the policy.</span></span> <span data-ttu-id="bfe13-121">Os valores possíveis são: `deviceConfiguration`, `deviceIntent`.</span><span class="sxs-lookup"><span data-stu-id="bfe13-121">Possible values are: `deviceConfiguration`, `deviceIntent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfe13-122">Relações</span><span class="sxs-lookup"><span data-stu-id="bfe13-122">Relationships</span></span>
<span data-ttu-id="bfe13-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bfe13-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfe13-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bfe13-124">JSON Representation</span></span>
<span data-ttu-id="bfe13-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bfe13-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.securityBaselineContributingPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineContributingPolicy",
  "sourceId": "String",
  "displayName": "String",
  "sourceType": "String"
}
```




