---
title: tipo de recurso educationSynchronizationProfileStatus
description: 'Representa o status de sincronização de um perfil de sincronização de dados da escola. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2ba9b9d8ecf6766cddfa670ae2e33b39d0e6acb6
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434869"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="f160b-103">tipo de recurso educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="f160b-103">educationSynchronizationProfileStatus resource type</span></span>

<span data-ttu-id="f160b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f160b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f160b-105">Representa o status de sincronização de um [perfil de sincronização](educationsynchronizationprofile.md)de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="f160b-105">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span>

> <span data-ttu-id="f160b-106">**Observação:** As atualizações do **educationSynchronizationProfileStatus** podem ser atrasadas devido à natureza assíncrona do processamento de sincronização em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="f160b-106">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="f160b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="f160b-107">Methods</span></span>

| <span data-ttu-id="f160b-108">Método</span><span class="sxs-lookup"><span data-stu-id="f160b-108">Method</span></span>                                                                      | <span data-ttu-id="f160b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f160b-109">Return Type</span></span>                               | <span data-ttu-id="f160b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f160b-110">Description</span></span>                                              |
| :-------------------------------------------------------------------------- | :---------------------------------------- | :------------------------------------------------------- |
| [<span data-ttu-id="f160b-111">Obter o status de uma sincronização</span><span class="sxs-lookup"><span data-stu-id="f160b-111">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="f160b-112">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="f160b-112">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="f160b-113">Retornar o status de um perfil de sincronização específico.</span><span class="sxs-lookup"><span data-stu-id="f160b-113">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="f160b-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f160b-114">Properties</span></span>

| <span data-ttu-id="f160b-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f160b-115">Property</span></span>                    | <span data-ttu-id="f160b-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="f160b-116">Type</span></span>                           | <span data-ttu-id="f160b-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f160b-117">Description</span></span>                                                                                                              |
| :-------------------------- | :----------------------------- | :----------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f160b-118">id</span><span class="sxs-lookup"><span data-stu-id="f160b-118">id</span></span>                          | <span data-ttu-id="f160b-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f160b-119">String</span></span>                         | <span data-ttu-id="f160b-120">O identificador exclusivo do recurso.</span><span class="sxs-lookup"><span data-stu-id="f160b-120">The unique identifier for the resource.</span></span> <span data-ttu-id="f160b-121">(somente leitura)</span><span class="sxs-lookup"><span data-stu-id="f160b-121">(read-only)</span></span>                                                                      |
| <span data-ttu-id="f160b-122">status</span><span class="sxs-lookup"><span data-stu-id="f160b-122">status</span></span>                      | <span data-ttu-id="f160b-123">educationSynchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="f160b-123">educationSynchronizationStatus</span></span> | <span data-ttu-id="f160b-124">O status de uma sincronização. Os valores possíveis são: `paused` , `inProgress` , `success` , `error` , `quarantined` , `validationError` .</span><span class="sxs-lookup"><span data-stu-id="f160b-124">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="f160b-125">lastSynchronizationDateTime</span><span class="sxs-lookup"><span data-stu-id="f160b-125">lastSynchronizationDateTime</span></span> | <span data-ttu-id="f160b-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f160b-126">DateTimeOffset</span></span>                 | <span data-ttu-id="f160b-127">Representa a hora em que as alterações mais recentes foram observadas no diretório.</span><span class="sxs-lookup"><span data-stu-id="f160b-127">Represents the time when most recent changes have been observed in the directory.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="f160b-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f160b-128">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
  "id": "String",
  "status": { "@odata.type": "microsoft.graph.educationSynchronizationStatus" },
  "lastSynchronizationDateTime": "DateTimeOffset"
}
```
