---
title: tipo de recurso encryptionReportPolicyDetails
description: Detalhes da política para o relatório de criptografia
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ddca213c3de3c004a19ebc3877aed1542604933e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946641"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="e4fad-103">tipo de recurso encryptionReportPolicyDetails</span><span class="sxs-lookup"><span data-stu-id="e4fad-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="e4fad-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4fad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4fad-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4fad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4fad-106">Detalhes da política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="e4fad-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="e4fad-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e4fad-107">Properties</span></span>
|<span data-ttu-id="e4fad-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4fad-108">Property</span></span>|<span data-ttu-id="e4fad-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4fad-109">Type</span></span>|<span data-ttu-id="e4fad-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4fad-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4fad-111">PolicyId</span><span class="sxs-lookup"><span data-stu-id="e4fad-111">policyId</span></span>|<span data-ttu-id="e4fad-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4fad-112">String</span></span>|<span data-ttu-id="e4fad-113">ID de política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="e4fad-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="e4fad-114">policyName</span><span class="sxs-lookup"><span data-stu-id="e4fad-114">policyName</span></span>|<span data-ttu-id="e4fad-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4fad-115">String</span></span>|<span data-ttu-id="e4fad-116">Nome da política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="e4fad-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4fad-117">Relações</span><span class="sxs-lookup"><span data-stu-id="e4fad-117">Relationships</span></span>
<span data-ttu-id="e4fad-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e4fad-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4fad-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4fad-119">JSON Representation</span></span>
<span data-ttu-id="e4fad-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e4fad-120">Here is a JSON representation of the resource.</span></span>
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




