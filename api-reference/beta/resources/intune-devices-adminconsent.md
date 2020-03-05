---
title: tipo de recurso adminConsent
description: Informações de consentimento do administrador.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d9b6e3ce006c78d2f83406fe9fe7e4092089339
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525184"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="5502d-103">tipo de recurso adminConsent</span><span class="sxs-lookup"><span data-stu-id="5502d-103">adminConsent resource type</span></span>

<span data-ttu-id="5502d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5502d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5502d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5502d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5502d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5502d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5502d-107">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="5502d-107">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="5502d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5502d-108">Properties</span></span>
|<span data-ttu-id="5502d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5502d-109">Property</span></span>|<span data-ttu-id="5502d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5502d-110">Type</span></span>|<span data-ttu-id="5502d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5502d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5502d-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="5502d-112">shareAPNSData</span></span>|[<span data-ttu-id="5502d-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="5502d-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="5502d-114">O estado de consentimento do administrador do compartilhamento de dados de usuário e de dispositivo para a Apple.</span><span class="sxs-lookup"><span data-stu-id="5502d-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="5502d-115">Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="5502d-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|
|<span data-ttu-id="5502d-116">shareUserExperienceAnalyticsData</span><span class="sxs-lookup"><span data-stu-id="5502d-116">shareUserExperienceAnalyticsData</span></span>|[<span data-ttu-id="5502d-117">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="5502d-117">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="5502d-118">Obtém ou define o consentimento do administrador para compartilhamento de dados da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="5502d-118">Gets or sets the admin consent for sharing User experience analytics data.</span></span> <span data-ttu-id="5502d-119">Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="5502d-119">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5502d-120">Relações</span><span class="sxs-lookup"><span data-stu-id="5502d-120">Relationships</span></span>
<span data-ttu-id="5502d-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5502d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5502d-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5502d-122">JSON Representation</span></span>
<span data-ttu-id="5502d-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5502d-123">Here is a JSON representation of the resource.</span></span>
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



