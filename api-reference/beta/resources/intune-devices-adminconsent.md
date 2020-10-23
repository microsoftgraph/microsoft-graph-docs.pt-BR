---
title: tipo de recurso adminConsent
description: Informações de consentimento do administrador.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3382670e9c5b00f37970aa385ad508fd8003ee7d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725565"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="98948-103">tipo de recurso adminConsent</span><span class="sxs-lookup"><span data-stu-id="98948-103">adminConsent resource type</span></span>

<span data-ttu-id="98948-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98948-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98948-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="98948-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98948-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="98948-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98948-107">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="98948-107">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="98948-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98948-108">Properties</span></span>
|<span data-ttu-id="98948-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98948-109">Property</span></span>|<span data-ttu-id="98948-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="98948-110">Type</span></span>|<span data-ttu-id="98948-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="98948-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98948-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="98948-112">shareAPNSData</span></span>|[<span data-ttu-id="98948-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="98948-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="98948-114">O estado de consentimento do administrador do compartilhamento de dados de usuário e de dispositivo para a Apple.</span><span class="sxs-lookup"><span data-stu-id="98948-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="98948-115">Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="98948-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|
|<span data-ttu-id="98948-116">shareUserExperienceAnalyticsData</span><span class="sxs-lookup"><span data-stu-id="98948-116">shareUserExperienceAnalyticsData</span></span>|[<span data-ttu-id="98948-117">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="98948-117">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="98948-118">Obtém ou define o consentimento do administrador para compartilhamento de dados da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="98948-118">Gets or sets the admin consent for sharing User experience analytics data.</span></span> <span data-ttu-id="98948-119">Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="98948-119">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98948-120">Relações</span><span class="sxs-lookup"><span data-stu-id="98948-120">Relationships</span></span>
<span data-ttu-id="98948-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="98948-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98948-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98948-122">JSON Representation</span></span>
<span data-ttu-id="98948-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="98948-123">Here is a JSON representation of the resource.</span></span>
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





