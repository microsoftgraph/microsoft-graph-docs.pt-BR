---
title: tipo de recurso de deviceManagementTroubleshootingErrorDetails
description: Objeto que contém informações detalhadas sobre o erro e suas atualizações.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9cdda64170afc739c23f1b258e5f2f1b31158662
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429038"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="be983-103">tipo de recurso de deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="be983-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

> <span data-ttu-id="be983-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="be983-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="be983-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="be983-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be983-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="be983-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be983-107">Objeto que contém informações detalhadas sobre o erro e suas atualizações.</span><span class="sxs-lookup"><span data-stu-id="be983-107">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="be983-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be983-108">Properties</span></span>
|<span data-ttu-id="be983-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be983-109">Property</span></span>|<span data-ttu-id="be983-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="be983-110">Type</span></span>|<span data-ttu-id="be983-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="be983-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be983-112">context</span><span class="sxs-lookup"><span data-stu-id="be983-112">context</span></span>|<span data-ttu-id="be983-113">String</span><span class="sxs-lookup"><span data-stu-id="be983-113">String</span></span>|<span data-ttu-id="be983-114">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="be983-114">Not yet documented</span></span>|
|<span data-ttu-id="be983-115">Falha</span><span class="sxs-lookup"><span data-stu-id="be983-115">failure</span></span>|<span data-ttu-id="be983-116">String</span><span class="sxs-lookup"><span data-stu-id="be983-116">String</span></span>|<span data-ttu-id="be983-117">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="be983-117">Not yet documented</span></span>|
|<span data-ttu-id="be983-118">failureDetails</span><span class="sxs-lookup"><span data-stu-id="be983-118">failureDetails</span></span>|<span data-ttu-id="be983-119">String</span><span class="sxs-lookup"><span data-stu-id="be983-119">String</span></span>|<span data-ttu-id="be983-120">A descrição detalhada do que deu errada.</span><span class="sxs-lookup"><span data-stu-id="be983-120">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="be983-121">remediação</span><span class="sxs-lookup"><span data-stu-id="be983-121">remediation</span></span>|<span data-ttu-id="be983-122">String</span><span class="sxs-lookup"><span data-stu-id="be983-122">String</span></span>|<span data-ttu-id="be983-123">A descrição detalhada de como corrigir esse problema.</span><span class="sxs-lookup"><span data-stu-id="be983-123">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="be983-124">recursos</span><span class="sxs-lookup"><span data-stu-id="be983-124">resources</span></span>|<span data-ttu-id="be983-125">coleção [deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)</span><span class="sxs-lookup"><span data-stu-id="be983-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="be983-126">Links para documentação úteis sobre essa falha.</span><span class="sxs-lookup"><span data-stu-id="be983-126">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be983-127">Relações</span><span class="sxs-lookup"><span data-stu-id="be983-127">Relationships</span></span>
<span data-ttu-id="be983-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="be983-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be983-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be983-129">JSON Representation</span></span>
<span data-ttu-id="be983-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="be983-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorDetails",
  "context": "String",
  "failure": "String",
  "failureDetails": "String",
  "remediation": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
      "text": "String",
      "link": "String"
    }
  ]
}
```




