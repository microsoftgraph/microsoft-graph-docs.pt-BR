---
title: tipo de recurso encryptionReportPolicyDetails
description: Detalhes da política para o relatório de criptografia
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c9903b54483fc6f77cd183abee0e54b10acf9cc
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771009"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="2ad79-103">tipo de recurso encryptionReportPolicyDetails</span><span class="sxs-lookup"><span data-stu-id="2ad79-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="2ad79-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ad79-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ad79-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ad79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ad79-106">Detalhes da política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="2ad79-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="2ad79-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ad79-107">Properties</span></span>
|<span data-ttu-id="2ad79-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ad79-108">Property</span></span>|<span data-ttu-id="2ad79-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ad79-109">Type</span></span>|<span data-ttu-id="2ad79-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ad79-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ad79-111">PolicyId</span><span class="sxs-lookup"><span data-stu-id="2ad79-111">policyId</span></span>|<span data-ttu-id="2ad79-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ad79-112">String</span></span>|<span data-ttu-id="2ad79-113">ID de política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="2ad79-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="2ad79-114">policyName</span><span class="sxs-lookup"><span data-stu-id="2ad79-114">policyName</span></span>|<span data-ttu-id="2ad79-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ad79-115">String</span></span>|<span data-ttu-id="2ad79-116">Nome da política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="2ad79-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ad79-117">Relações</span><span class="sxs-lookup"><span data-stu-id="2ad79-117">Relationships</span></span>
<span data-ttu-id="2ad79-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2ad79-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ad79-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ad79-119">JSON Representation</span></span>
<span data-ttu-id="2ad79-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ad79-120">Here is a JSON representation of the resource.</span></span>
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





