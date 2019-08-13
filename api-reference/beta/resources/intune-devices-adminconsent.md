---
title: tipo de recurso adminConsent
description: Informações de consentimento do administrador.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8d78333cd683501a8bf4fea0aa3a2e55944d9b5a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319304"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="f99ac-103">tipo de recurso adminConsent</span><span class="sxs-lookup"><span data-stu-id="f99ac-103">adminConsent resource type</span></span>

> <span data-ttu-id="f99ac-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f99ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f99ac-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f99ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f99ac-106">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="f99ac-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="f99ac-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f99ac-107">Properties</span></span>
|<span data-ttu-id="f99ac-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f99ac-108">Property</span></span>|<span data-ttu-id="f99ac-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f99ac-109">Type</span></span>|<span data-ttu-id="f99ac-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f99ac-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f99ac-111">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="f99ac-111">shareAPNSData</span></span>|[<span data-ttu-id="f99ac-112">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="f99ac-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="f99ac-113">O estado de consentimento do administrador do compartilhamento de dados de usuário e de dispositivo para a Apple.</span><span class="sxs-lookup"><span data-stu-id="f99ac-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="f99ac-114">Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="f99ac-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|
|<span data-ttu-id="f99ac-115">shareUserExperienceAnalyticsData</span><span class="sxs-lookup"><span data-stu-id="f99ac-115">shareUserExperienceAnalyticsData</span></span>|[<span data-ttu-id="f99ac-116">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="f99ac-116">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="f99ac-117">Obtém ou define o consentimento do administrador para compartilhamento de dados da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="f99ac-117">Gets or sets the admin consent for sharing User experience analytics data.</span></span> <span data-ttu-id="f99ac-118">Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="f99ac-118">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f99ac-119">Relações</span><span class="sxs-lookup"><span data-stu-id="f99ac-119">Relationships</span></span>
<span data-ttu-id="f99ac-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f99ac-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f99ac-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f99ac-121">JSON Representation</span></span>
<span data-ttu-id="f99ac-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f99ac-122">Here is a JSON representation of the resource.</span></span>
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



