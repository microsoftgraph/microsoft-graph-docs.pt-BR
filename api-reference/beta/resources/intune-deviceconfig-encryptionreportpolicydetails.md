---
title: tipo de recurso encryptionReportPolicyDetails
description: Detalhes da política para o relatório de criptografia
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8a92037429908af4ff53ea45b9b5f9b65a5a436
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460062"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="3997a-103">tipo de recurso encryptionReportPolicyDetails</span><span class="sxs-lookup"><span data-stu-id="3997a-103">encryptionReportPolicyDetails resource type</span></span>

<span data-ttu-id="3997a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3997a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3997a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3997a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3997a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3997a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3997a-107">Detalhes da política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="3997a-107">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="3997a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3997a-108">Properties</span></span>
|<span data-ttu-id="3997a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3997a-109">Property</span></span>|<span data-ttu-id="3997a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3997a-110">Type</span></span>|<span data-ttu-id="3997a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3997a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3997a-112">PolicyId</span><span class="sxs-lookup"><span data-stu-id="3997a-112">policyId</span></span>|<span data-ttu-id="3997a-113">String</span><span class="sxs-lookup"><span data-stu-id="3997a-113">String</span></span>|<span data-ttu-id="3997a-114">ID de política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="3997a-114">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="3997a-115">policyName</span><span class="sxs-lookup"><span data-stu-id="3997a-115">policyName</span></span>|<span data-ttu-id="3997a-116">String</span><span class="sxs-lookup"><span data-stu-id="3997a-116">String</span></span>|<span data-ttu-id="3997a-117">Nome da política para o relatório de criptografia</span><span class="sxs-lookup"><span data-stu-id="3997a-117">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="3997a-118">Relações</span><span class="sxs-lookup"><span data-stu-id="3997a-118">Relationships</span></span>
<span data-ttu-id="3997a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3997a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3997a-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3997a-120">JSON Representation</span></span>
<span data-ttu-id="3997a-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3997a-121">Here is a JSON representation of the resource.</span></span>
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



