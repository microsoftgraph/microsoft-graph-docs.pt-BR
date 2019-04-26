---
title: tipo de recurso encryptionReportPolicyDetails
description: Detalhes da política para o relatório de criptografia
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c9903b54483fc6f77cd183abee0e54b10acf9cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556295"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="391aa-103">tipo de recurso encryptionReportPolicyDetails</span><span class="sxs-lookup"><span data-stu-id="391aa-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="391aa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="391aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="391aa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="391aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="391aa-106">Detalhes da política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="391aa-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="391aa-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="391aa-107">Properties</span></span>
|<span data-ttu-id="391aa-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="391aa-108">Property</span></span>|<span data-ttu-id="391aa-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="391aa-109">Type</span></span>|<span data-ttu-id="391aa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="391aa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="391aa-111">PolicyId</span><span class="sxs-lookup"><span data-stu-id="391aa-111">policyId</span></span>|<span data-ttu-id="391aa-112">String</span><span class="sxs-lookup"><span data-stu-id="391aa-112">String</span></span>|<span data-ttu-id="391aa-113">ID de política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="391aa-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="391aa-114">policyName</span><span class="sxs-lookup"><span data-stu-id="391aa-114">policyName</span></span>|<span data-ttu-id="391aa-115">String</span><span class="sxs-lookup"><span data-stu-id="391aa-115">String</span></span>|<span data-ttu-id="391aa-116">Nome da política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="391aa-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="391aa-117">Relações</span><span class="sxs-lookup"><span data-stu-id="391aa-117">Relationships</span></span>
<span data-ttu-id="391aa-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="391aa-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="391aa-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="391aa-119">JSON Representation</span></span>
<span data-ttu-id="391aa-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="391aa-120">Here is a JSON representation of the resource.</span></span>
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





