---
title: tipo de recurso de educationSynchronizationProfileStatus
description: 'Representa o status da sincronização de um perfil de sincronização de dados escola. '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 4476ffc7c64fb5d9852c46e2b748587e79d427c1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858160"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="82183-103">tipo de recurso de educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="82183-103">educationSynchronizationProfileStatus resource type</span></span>

> <span data-ttu-id="82183-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="82183-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82183-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="82183-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="82183-106">Representa o status da sincronização de um [perfil de sincronização](educationsynchronizationprofile.md)de dados do escola.</span><span class="sxs-lookup"><span data-stu-id="82183-106">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="82183-107">**Observação:** Atualizações para o **educationSynchronizationProfileStatus** podem ser atrasadas devido a natureza assíncrona do processamento de sincronização em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="82183-107">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="82183-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="82183-108">Methods</span></span>

| <span data-ttu-id="82183-109">Método</span><span class="sxs-lookup"><span data-stu-id="82183-109">Method</span></span> | <span data-ttu-id="82183-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="82183-110">Return Type</span></span> | <span data-ttu-id="82183-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="82183-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="82183-112">Obter o status de uma sincronização</span><span class="sxs-lookup"><span data-stu-id="82183-112">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="82183-113">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="82183-113">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="82183-114">Retorna o status de um perfil de sincronização específico.</span><span class="sxs-lookup"><span data-stu-id="82183-114">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="82183-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82183-115">Properties</span></span>

| <span data-ttu-id="82183-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82183-116">Property</span></span> | <span data-ttu-id="82183-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="82183-117">Type</span></span> | <span data-ttu-id="82183-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="82183-118">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="82183-119">**status**</span><span class="sxs-lookup"><span data-stu-id="82183-119">**status**</span></span> | <span data-ttu-id="82183-120">string</span><span class="sxs-lookup"><span data-stu-id="82183-120">string</span></span> | <span data-ttu-id="82183-121">O status de uma sincronização. Os valores possíveis são: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span><span class="sxs-lookup"><span data-stu-id="82183-121">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="82183-122">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="82183-122">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="82183-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82183-123">DateTimeOffset</span></span> | <span data-ttu-id="82183-124">Representa a hora quando as alterações mais recentes têm foi observadas no diretório.</span><span class="sxs-lookup"><span data-stu-id="82183-124">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="82183-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82183-125">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```
