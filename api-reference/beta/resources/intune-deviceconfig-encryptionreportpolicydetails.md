---
title: tipo de recurso encryptionReportPolicyDetails
description: Detalhes da política para o relatório de criptografia
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd802c6a13789f9179d4f2940bc78a80f1ff15d0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791783"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="89196-103">tipo de recurso encryptionReportPolicyDetails</span><span class="sxs-lookup"><span data-stu-id="89196-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="89196-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89196-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89196-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89196-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89196-106">Detalhes da política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="89196-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="89196-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89196-107">Properties</span></span>
|<span data-ttu-id="89196-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89196-108">Property</span></span>|<span data-ttu-id="89196-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="89196-109">Type</span></span>|<span data-ttu-id="89196-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="89196-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89196-111">PolicyId</span><span class="sxs-lookup"><span data-stu-id="89196-111">policyId</span></span>|<span data-ttu-id="89196-112">String</span><span class="sxs-lookup"><span data-stu-id="89196-112">String</span></span>|<span data-ttu-id="89196-113">ID de política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="89196-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="89196-114">policyName</span><span class="sxs-lookup"><span data-stu-id="89196-114">policyName</span></span>|<span data-ttu-id="89196-115">String</span><span class="sxs-lookup"><span data-stu-id="89196-115">String</span></span>|<span data-ttu-id="89196-116">Nome da política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="89196-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="89196-117">Relações</span><span class="sxs-lookup"><span data-stu-id="89196-117">Relationships</span></span>
<span data-ttu-id="89196-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89196-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89196-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89196-119">JSON Representation</span></span>
<span data-ttu-id="89196-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89196-120">Here is a JSON representation of the resource.</span></span>
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



