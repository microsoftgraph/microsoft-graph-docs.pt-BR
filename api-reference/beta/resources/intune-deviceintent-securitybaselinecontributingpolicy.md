---
title: tipo de recurso securityBaselineContributingPolicy
description: O estado de conformidade da linha de base de segurança de uma configuração para um dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0702786afdd049b28fd67638f4fe76920164c35
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704910"
---
# <a name="securitybaselinecontributingpolicy-resource-type"></a><span data-ttu-id="3ca90-103">tipo de recurso securityBaselineContributingPolicy</span><span class="sxs-lookup"><span data-stu-id="3ca90-103">securityBaselineContributingPolicy resource type</span></span>

<span data-ttu-id="3ca90-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ca90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ca90-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3ca90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ca90-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ca90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ca90-107">O estado de conformidade da linha de base de segurança de uma configuração para um dispositivo</span><span class="sxs-lookup"><span data-stu-id="3ca90-107">The security baseline compliance state of a setting for a device</span></span>

## <a name="properties"></a><span data-ttu-id="3ca90-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ca90-108">Properties</span></span>
|<span data-ttu-id="3ca90-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ca90-109">Property</span></span>|<span data-ttu-id="3ca90-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ca90-110">Type</span></span>|<span data-ttu-id="3ca90-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ca90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ca90-112">sourceId</span><span class="sxs-lookup"><span data-stu-id="3ca90-112">sourceId</span></span>|<span data-ttu-id="3ca90-113">String</span><span class="sxs-lookup"><span data-stu-id="3ca90-113">String</span></span>|<span data-ttu-id="3ca90-114">Identificador exclusivo da política</span><span class="sxs-lookup"><span data-stu-id="3ca90-114">Unique identifier of the policy</span></span>|
|<span data-ttu-id="3ca90-115">displayName</span><span class="sxs-lookup"><span data-stu-id="3ca90-115">displayName</span></span>|<span data-ttu-id="3ca90-116">String</span><span class="sxs-lookup"><span data-stu-id="3ca90-116">String</span></span>|<span data-ttu-id="3ca90-117">Nome da política</span><span class="sxs-lookup"><span data-stu-id="3ca90-117">Name of the policy</span></span>|
|<span data-ttu-id="3ca90-118">sourceType</span><span class="sxs-lookup"><span data-stu-id="3ca90-118">sourceType</span></span>|[<span data-ttu-id="3ca90-119">securityBaselinePolicySourceType</span><span class="sxs-lookup"><span data-stu-id="3ca90-119">securityBaselinePolicySourceType</span></span>](../resources/intune-deviceintent-securitybaselinepolicysourcetype.md)|<span data-ttu-id="3ca90-120">Fonte de criação da política.</span><span class="sxs-lookup"><span data-stu-id="3ca90-120">Authoring source of the policy.</span></span> <span data-ttu-id="3ca90-121">Os valores possíveis são: `deviceConfiguration`, `deviceIntent`.</span><span class="sxs-lookup"><span data-stu-id="3ca90-121">Possible values are: `deviceConfiguration`, `deviceIntent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ca90-122">Relações</span><span class="sxs-lookup"><span data-stu-id="3ca90-122">Relationships</span></span>
<span data-ttu-id="3ca90-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3ca90-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ca90-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ca90-124">JSON Representation</span></span>
<span data-ttu-id="3ca90-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3ca90-125">Here is a JSON representation of the resource.</span></span>
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





