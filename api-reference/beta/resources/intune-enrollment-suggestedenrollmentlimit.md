---
title: tipo de recurso suggestedEnrollmentLimit
description: O recurso suggestedEnrollmentLimit representa o limite de inscrição sugerido quando é atribuído um tipo de registro.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b54c89a946f6a5b5b8dd66a8e4146f6e12793d89
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728883"
---
# <a name="suggestedenrollmentlimit-resource-type"></a><span data-ttu-id="4ad72-103">tipo de recurso suggestedEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="4ad72-103">suggestedEnrollmentLimit resource type</span></span>

<span data-ttu-id="4ad72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ad72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ad72-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ad72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ad72-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ad72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ad72-107">O recurso suggestedEnrollmentLimit representa o limite de inscrição sugerido quando é atribuído um tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="4ad72-107">The suggestedEnrollmentLimit resource represents the suggested enrollment limit when given an enrollment type.</span></span>

## <a name="properties"></a><span data-ttu-id="4ad72-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ad72-108">Properties</span></span>
|<span data-ttu-id="4ad72-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ad72-109">Property</span></span>|<span data-ttu-id="4ad72-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ad72-110">Type</span></span>|<span data-ttu-id="4ad72-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ad72-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ad72-112">suggestedDailyLimit</span><span class="sxs-lookup"><span data-stu-id="4ad72-112">suggestedDailyLimit</span></span>|<span data-ttu-id="4ad72-113">Int32</span><span class="sxs-lookup"><span data-stu-id="4ad72-113">Int32</span></span>|<span data-ttu-id="4ad72-114">O limite de inscrição sugerido dentro de um dia</span><span class="sxs-lookup"><span data-stu-id="4ad72-114">The suggested enrollment limit within a day</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ad72-115">Relações</span><span class="sxs-lookup"><span data-stu-id="4ad72-115">Relationships</span></span>
<span data-ttu-id="4ad72-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ad72-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ad72-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ad72-117">JSON Representation</span></span>
<span data-ttu-id="4ad72-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ad72-118">Here is a JSON representation of the resource.</span></span>
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





