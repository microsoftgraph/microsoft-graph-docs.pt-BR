---
title: tipo de recurso suggestedEnrollmentLimit
description: O recurso suggestedEnrollmentLimit representa o limite de inscrição sugerido quando é atribuído um tipo de registro.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 880fb5d77c7fa16a23349918973a33ba0952e07a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256257"
---
# <a name="suggestedenrollmentlimit-resource-type"></a><span data-ttu-id="bc386-103">tipo de recurso suggestedEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="bc386-103">suggestedEnrollmentLimit resource type</span></span>

<span data-ttu-id="bc386-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc386-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc386-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc386-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc386-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc386-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc386-107">O recurso suggestedEnrollmentLimit representa o limite de inscrição sugerido quando é atribuído um tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="bc386-107">The suggestedEnrollmentLimit resource represents the suggested enrollment limit when given an enrollment type.</span></span>

## <a name="properties"></a><span data-ttu-id="bc386-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc386-108">Properties</span></span>
|<span data-ttu-id="bc386-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc386-109">Property</span></span>|<span data-ttu-id="bc386-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc386-110">Type</span></span>|<span data-ttu-id="bc386-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc386-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc386-112">suggestedDailyLimit</span><span class="sxs-lookup"><span data-stu-id="bc386-112">suggestedDailyLimit</span></span>|<span data-ttu-id="bc386-113">Int32</span><span class="sxs-lookup"><span data-stu-id="bc386-113">Int32</span></span>|<span data-ttu-id="bc386-114">O limite de inscrição sugerido dentro de um dia</span><span class="sxs-lookup"><span data-stu-id="bc386-114">The suggested enrollment limit within a day</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc386-115">Relações</span><span class="sxs-lookup"><span data-stu-id="bc386-115">Relationships</span></span>
<span data-ttu-id="bc386-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc386-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc386-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc386-117">JSON Representation</span></span>
<span data-ttu-id="bc386-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc386-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.suggestedEnrollmentLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.suggestedEnrollmentLimit",
  "suggestedDailyLimit": 1024
}
```




