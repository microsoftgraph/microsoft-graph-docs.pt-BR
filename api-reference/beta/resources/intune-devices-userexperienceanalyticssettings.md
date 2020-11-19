---
title: tipo de recurso userExperienceAnalyticsSettings
description: A visão geral da análise da experiência do usuário é a recomendação de melhorar a pontuação de análise da experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 38ef61cf5204b41aa0507bf164e6e8abf0508d90
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259974"
---
# <a name="userexperienceanalyticssettings-resource-type"></a><span data-ttu-id="00bde-103">tipo de recurso userExperienceAnalyticsSettings</span><span class="sxs-lookup"><span data-stu-id="00bde-103">userExperienceAnalyticsSettings resource type</span></span>

<span data-ttu-id="00bde-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00bde-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00bde-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="00bde-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00bde-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00bde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00bde-107">A visão geral da análise da experiência do usuário é a recomendação de melhorar a pontuação de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="00bde-107">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="00bde-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00bde-108">Properties</span></span>
|<span data-ttu-id="00bde-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00bde-109">Property</span></span>|<span data-ttu-id="00bde-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="00bde-110">Type</span></span>|<span data-ttu-id="00bde-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="00bde-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00bde-112">configurationManagerDataConnectorConfigured</span><span class="sxs-lookup"><span data-stu-id="00bde-112">configurationManagerDataConnectorConfigured</span></span>|<span data-ttu-id="00bde-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="00bde-113">Boolean</span></span>|<span data-ttu-id="00bde-114">True se o anexo do locatário estiver configurado.</span><span class="sxs-lookup"><span data-stu-id="00bde-114">True if Tenant attach is configured.</span></span> <span data-ttu-id="00bde-115">Se configurado, os dispositivos anexados ao locatário do SCCM aparecerão nos relatórios do UXA.</span><span class="sxs-lookup"><span data-stu-id="00bde-115">If configured then SCCM tenant attached devices will show up in UXA reporting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00bde-116">Relações</span><span class="sxs-lookup"><span data-stu-id="00bde-116">Relationships</span></span>
<span data-ttu-id="00bde-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="00bde-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00bde-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00bde-118">JSON Representation</span></span>
<span data-ttu-id="00bde-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00bde-119">Here is a JSON representation of the resource.</span></span>
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




