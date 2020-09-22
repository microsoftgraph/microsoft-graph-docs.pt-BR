---
title: tipo de recurso suggestedEnrollmentLimit
description: O recurso suggestedEnrollmentLimit representa o limite de inscrição sugerido quando é atribuído um tipo de registro.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 99efb75bcf52b841dcf67741045b7207a85eb3cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081957"
---
# <a name="suggestedenrollmentlimit-resource-type"></a><span data-ttu-id="6fac5-103">tipo de recurso suggestedEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="6fac5-103">suggestedEnrollmentLimit resource type</span></span>

<span data-ttu-id="6fac5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fac5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fac5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6fac5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fac5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6fac5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fac5-107">O recurso suggestedEnrollmentLimit representa o limite de inscrição sugerido quando é atribuído um tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="6fac5-107">The suggestedEnrollmentLimit resource represents the suggested enrollment limit when given an enrollment type.</span></span>

## <a name="properties"></a><span data-ttu-id="6fac5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6fac5-108">Properties</span></span>
|<span data-ttu-id="6fac5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fac5-109">Property</span></span>|<span data-ttu-id="6fac5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fac5-110">Type</span></span>|<span data-ttu-id="6fac5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fac5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fac5-112">suggestedDailyLimit</span><span class="sxs-lookup"><span data-stu-id="6fac5-112">suggestedDailyLimit</span></span>|<span data-ttu-id="6fac5-113">Int32</span><span class="sxs-lookup"><span data-stu-id="6fac5-113">Int32</span></span>|<span data-ttu-id="6fac5-114">O limite de inscrição sugerido dentro de um dia</span><span class="sxs-lookup"><span data-stu-id="6fac5-114">The suggested enrollment limit within a day</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fac5-115">Relações</span><span class="sxs-lookup"><span data-stu-id="6fac5-115">Relationships</span></span>
<span data-ttu-id="6fac5-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6fac5-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fac5-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6fac5-117">JSON Representation</span></span>
<span data-ttu-id="6fac5-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6fac5-118">Here is a JSON representation of the resource.</span></span>
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






