---
title: tipo de recurso userExperienceAnalyticsSettings
description: A visão geral da análise da experiência do usuário é a recomendação de melhorar a pontuação de análise da experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 950bd227d36cc691072fb11b17d2a0972d00de07
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793644"
---
# <a name="userexperienceanalyticssettings-resource-type"></a><span data-ttu-id="faca7-103">tipo de recurso userExperienceAnalyticsSettings</span><span class="sxs-lookup"><span data-stu-id="faca7-103">userExperienceAnalyticsSettings resource type</span></span>

<span data-ttu-id="faca7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="faca7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="faca7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="faca7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="faca7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="faca7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faca7-107">A visão geral da análise da experiência do usuário é a recomendação de melhorar a pontuação de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="faca7-107">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="faca7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="faca7-108">Properties</span></span>
|<span data-ttu-id="faca7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="faca7-109">Property</span></span>|<span data-ttu-id="faca7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="faca7-110">Type</span></span>|<span data-ttu-id="faca7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="faca7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faca7-112">configurationManagerDataConnectorConfigured</span><span class="sxs-lookup"><span data-stu-id="faca7-112">configurationManagerDataConnectorConfigured</span></span>|<span data-ttu-id="faca7-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="faca7-113">Boolean</span></span>|<span data-ttu-id="faca7-114">True se o anexo do locatário estiver configurado.</span><span class="sxs-lookup"><span data-stu-id="faca7-114">True if Tenant attach is configured.</span></span> <span data-ttu-id="faca7-115">Se configurado, os dispositivos anexados ao locatário do SCCM aparecerão nos relatórios do UXA.</span><span class="sxs-lookup"><span data-stu-id="faca7-115">If configured then SCCM tenant attached devices will show up in UXA reporting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="faca7-116">Relações</span><span class="sxs-lookup"><span data-stu-id="faca7-116">Relationships</span></span>
<span data-ttu-id="faca7-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="faca7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="faca7-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="faca7-118">JSON Representation</span></span>
<span data-ttu-id="faca7-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="faca7-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsSettings",
  "configurationManagerDataConnectorConfigured": true
}
```



