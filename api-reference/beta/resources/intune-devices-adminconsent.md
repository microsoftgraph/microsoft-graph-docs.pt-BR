---
title: tipo de recurso adminConsent
description: Informações de consentimento do administrador.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b09db43661113de84712a8228af047ca1683c383
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060899"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="fa091-103">tipo de recurso adminConsent</span><span class="sxs-lookup"><span data-stu-id="fa091-103">adminConsent resource type</span></span>

<span data-ttu-id="fa091-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa091-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa091-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fa091-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa091-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa091-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa091-107">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="fa091-107">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="fa091-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa091-108">Properties</span></span>
|<span data-ttu-id="fa091-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa091-109">Property</span></span>|<span data-ttu-id="fa091-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa091-110">Type</span></span>|<span data-ttu-id="fa091-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa091-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa091-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="fa091-112">shareAPNSData</span></span>|[<span data-ttu-id="fa091-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="fa091-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="fa091-114">O estado de consentimento do administrador do compartilhamento de dados de usuário e de dispositivo para a Apple.</span><span class="sxs-lookup"><span data-stu-id="fa091-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="fa091-115">Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="fa091-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|
|<span data-ttu-id="fa091-116">shareUserExperienceAnalyticsData</span><span class="sxs-lookup"><span data-stu-id="fa091-116">shareUserExperienceAnalyticsData</span></span>|[<span data-ttu-id="fa091-117">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="fa091-117">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="fa091-118">Obtém ou define o consentimento do administrador para compartilhamento de dados da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="fa091-118">Gets or sets the admin consent for sharing User experience analytics data.</span></span> <span data-ttu-id="fa091-119">Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="fa091-119">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa091-120">Relações</span><span class="sxs-lookup"><span data-stu-id="fa091-120">Relationships</span></span>
<span data-ttu-id="fa091-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fa091-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa091-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa091-122">JSON Representation</span></span>
<span data-ttu-id="fa091-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa091-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String",
  "shareUserExperienceAnalyticsData": "String"
}
```






