---
title: tipo de recurso encryptionReportPolicyDetails
description: Detalhes da política para o relatório de criptografia
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7271329a7536a6359bbc9662427e65e21ea39d8b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325607"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="12653-103">tipo de recurso encryptionReportPolicyDetails</span><span class="sxs-lookup"><span data-stu-id="12653-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="12653-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12653-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12653-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12653-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12653-106">Detalhes da política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="12653-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="12653-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12653-107">Properties</span></span>
|<span data-ttu-id="12653-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12653-108">Property</span></span>|<span data-ttu-id="12653-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="12653-109">Type</span></span>|<span data-ttu-id="12653-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="12653-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12653-111">PolicyId</span><span class="sxs-lookup"><span data-stu-id="12653-111">policyId</span></span>|<span data-ttu-id="12653-112">String</span><span class="sxs-lookup"><span data-stu-id="12653-112">String</span></span>|<span data-ttu-id="12653-113">ID de política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="12653-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="12653-114">policyName</span><span class="sxs-lookup"><span data-stu-id="12653-114">policyName</span></span>|<span data-ttu-id="12653-115">String</span><span class="sxs-lookup"><span data-stu-id="12653-115">String</span></span>|<span data-ttu-id="12653-116">Nome da política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="12653-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="12653-117">Relações</span><span class="sxs-lookup"><span data-stu-id="12653-117">Relationships</span></span>
<span data-ttu-id="12653-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12653-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="12653-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12653-119">JSON Representation</span></span>
<span data-ttu-id="12653-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12653-120">Here is a JSON representation of the resource.</span></span>
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



