---
title: tipo de recurso encryptionReportPolicyDetails
description: Detalhes da política para o relatório de criptografia
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4dd42ac3f80fae8e4946c72c856a0f560165584a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994187"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="652ac-103">tipo de recurso encryptionReportPolicyDetails</span><span class="sxs-lookup"><span data-stu-id="652ac-103">encryptionReportPolicyDetails resource type</span></span>

<span data-ttu-id="652ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="652ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="652ac-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="652ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="652ac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="652ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="652ac-107">Detalhes da política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="652ac-107">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="652ac-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="652ac-108">Properties</span></span>
|<span data-ttu-id="652ac-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="652ac-109">Property</span></span>|<span data-ttu-id="652ac-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="652ac-110">Type</span></span>|<span data-ttu-id="652ac-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="652ac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="652ac-112">PolicyId</span><span class="sxs-lookup"><span data-stu-id="652ac-112">policyId</span></span>|<span data-ttu-id="652ac-113">String</span><span class="sxs-lookup"><span data-stu-id="652ac-113">String</span></span>|<span data-ttu-id="652ac-114">ID de política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="652ac-114">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="652ac-115">policyName</span><span class="sxs-lookup"><span data-stu-id="652ac-115">policyName</span></span>|<span data-ttu-id="652ac-116">String</span><span class="sxs-lookup"><span data-stu-id="652ac-116">String</span></span>|<span data-ttu-id="652ac-117">Nome da política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="652ac-117">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="652ac-118">Relações</span><span class="sxs-lookup"><span data-stu-id="652ac-118">Relationships</span></span>
<span data-ttu-id="652ac-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="652ac-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="652ac-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="652ac-120">JSON Representation</span></span>
<span data-ttu-id="652ac-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="652ac-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.encryptionReportPolicyDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.encryptionReportPolicyDetails",
  "policyId": "String",
  "policyName": "String"
}
```






