---
title: Tipo de recurso appLogCollectionRequest
description: Entidade AppLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 44284785c3dacbed31d6b88960af23b50b0d48f2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133434"
---
# <a name="applogcollectionrequest-resource-type"></a><span data-ttu-id="d071b-103">Tipo de recurso appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="d071b-103">appLogCollectionRequest resource type</span></span>

<span data-ttu-id="d071b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d071b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d071b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d071b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d071b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d071b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d071b-107">Entidade AppLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="d071b-107">AppLogCollectionRequest Entity.</span></span>

## <a name="methods"></a><span data-ttu-id="d071b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d071b-108">Methods</span></span>
|<span data-ttu-id="d071b-109">Método</span><span class="sxs-lookup"><span data-stu-id="d071b-109">Method</span></span>|<span data-ttu-id="d071b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d071b-110">Return Type</span></span>|<span data-ttu-id="d071b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d071b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d071b-112">Obter appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="d071b-112">Get appLogCollectionRequest</span></span>](../api/intune-devices-applogcollectionrequest-get.md)|[<span data-ttu-id="d071b-113">appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="d071b-113">appLogCollectionRequest</span></span>](../resources/intune-devices-applogcollectionrequest.md)|<span data-ttu-id="d071b-114">Leia propriedades e relações do [objeto appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)</span><span class="sxs-lookup"><span data-stu-id="d071b-114">Read properties and relationships of the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>|
|[<span data-ttu-id="d071b-115">Criar appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="d071b-115">Create appLogCollectionRequest</span></span>](../api/intune-devices-applogcollectionrequest-create.md)|[<span data-ttu-id="d071b-116">appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="d071b-116">appLogCollectionRequest</span></span>](../resources/intune-devices-applogcollectionrequest.md)|<span data-ttu-id="d071b-117">Crie um novo [objeto appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)</span><span class="sxs-lookup"><span data-stu-id="d071b-117">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>|
|[<span data-ttu-id="d071b-118">ação createDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="d071b-118">createDownloadUrl action</span></span>](../api/intune-devices-applogcollectionrequest-createdownloadurl.md)|[<span data-ttu-id="d071b-119">appLogCollectionDownloadDetails</span><span class="sxs-lookup"><span data-stu-id="d071b-119">appLogCollectionDownloadDetails</span></span>](../resources/intune-devices-applogcollectiondownloaddetails.md)|<span data-ttu-id="d071b-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d071b-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d071b-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d071b-121">Properties</span></span>
|<span data-ttu-id="d071b-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d071b-122">Property</span></span>|<span data-ttu-id="d071b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="d071b-123">Type</span></span>|<span data-ttu-id="d071b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d071b-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d071b-125">id</span><span class="sxs-lookup"><span data-stu-id="d071b-125">id</span></span>|<span data-ttu-id="d071b-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d071b-126">String</span></span>|<span data-ttu-id="d071b-127">O Identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="d071b-127">The unique Identifier.</span></span> <span data-ttu-id="d071b-128">Esta é userId_DeviceId_AppId id.</span><span class="sxs-lookup"><span data-stu-id="d071b-128">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="d071b-129">status</span><span class="sxs-lookup"><span data-stu-id="d071b-129">status</span></span>|[<span data-ttu-id="d071b-130">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="d071b-130">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="d071b-131">Status do carregamento de log.</span><span class="sxs-lookup"><span data-stu-id="d071b-131">Log upload status.</span></span> <span data-ttu-id="d071b-132">Os valores possíveis são: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="d071b-132">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="d071b-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="d071b-133">errorMessage</span></span>|<span data-ttu-id="d071b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d071b-134">String</span></span>|<span data-ttu-id="d071b-135">Mensagem de erro se alguma durante o processo de carregamento</span><span class="sxs-lookup"><span data-stu-id="d071b-135">Error message if any during the upload process</span></span>|
|<span data-ttu-id="d071b-136">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="d071b-136">customLogFolders</span></span>|<span data-ttu-id="d071b-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d071b-137">String collection</span></span>|<span data-ttu-id="d071b-138">Lista de pastas de log.</span><span class="sxs-lookup"><span data-stu-id="d071b-138">List of log folders.</span></span> |
|<span data-ttu-id="d071b-139">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="d071b-139">completedDateTime</span></span>|<span data-ttu-id="d071b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d071b-140">DateTimeOffset</span></span>|<span data-ttu-id="d071b-141">Hora em que a solicitação de log de carregamento atingiu um estado de terminal</span><span class="sxs-lookup"><span data-stu-id="d071b-141">Time at which the upload log request reached a terminal state</span></span>|

## <a name="relationships"></a><span data-ttu-id="d071b-142">Relações</span><span class="sxs-lookup"><span data-stu-id="d071b-142">Relationships</span></span>
<span data-ttu-id="d071b-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d071b-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d071b-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d071b-144">JSON Representation</span></span>
<span data-ttu-id="d071b-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d071b-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appLogCollectionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "String (identifier)",
  "status": "String",
  "errorMessage": "String",
  "customLogFolders": [
    "String"
  ],
  "completedDateTime": "String (timestamp)"
}
```




