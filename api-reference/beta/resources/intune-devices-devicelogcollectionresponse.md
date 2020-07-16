---
title: tipo de recurso deviceLogCollectionResponse
description: Entidade de solicitação de conjunto de logs do Windows.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1f9b6dcfda30845138c4576b3a100b8fbe3ff26c
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124155"
---
# <a name="devicelogcollectionresponse-resource-type"></a><span data-ttu-id="1a184-103">tipo de recurso deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="1a184-103">deviceLogCollectionResponse resource type</span></span>

<span data-ttu-id="1a184-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a184-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a184-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1a184-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a184-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a184-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a184-107">Entidade de solicitação de conjunto de logs do Windows.</span><span class="sxs-lookup"><span data-stu-id="1a184-107">Windows Log Collection request entity.</span></span>

## <a name="methods"></a><span data-ttu-id="1a184-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="1a184-108">Methods</span></span>
|<span data-ttu-id="1a184-109">Método</span><span class="sxs-lookup"><span data-stu-id="1a184-109">Method</span></span>|<span data-ttu-id="1a184-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1a184-110">Return Type</span></span>|<span data-ttu-id="1a184-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a184-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1a184-112">Listar deviceLogCollectionResponses</span><span class="sxs-lookup"><span data-stu-id="1a184-112">List deviceLogCollectionResponses</span></span>](../api/intune-devices-devicelogcollectionresponse-list.md)|<span data-ttu-id="1a184-113">coleção [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="1a184-113">[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) collection</span></span>|<span data-ttu-id="1a184-114">Listar Propriedades e relações dos objetos [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="1a184-114">List properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) objects.</span></span>|
|[<span data-ttu-id="1a184-115">Obter deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="1a184-115">Get deviceLogCollectionResponse</span></span>](../api/intune-devices-devicelogcollectionresponse-get.md)|[<span data-ttu-id="1a184-116">deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="1a184-116">deviceLogCollectionResponse</span></span>](../resources/intune-devices-devicelogcollectionresponse.md)|<span data-ttu-id="1a184-117">Leia as propriedades e as relações do objeto [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="1a184-117">Read properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>|
|[<span data-ttu-id="1a184-118">ação createDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="1a184-118">createDownloadUrl action</span></span>](../api/intune-devices-devicelogcollectionresponse-createdownloadurl.md)|<span data-ttu-id="1a184-119">String</span><span class="sxs-lookup"><span data-stu-id="1a184-119">String</span></span>|<span data-ttu-id="1a184-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1a184-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1a184-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a184-121">Properties</span></span>
|<span data-ttu-id="1a184-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a184-122">Property</span></span>|<span data-ttu-id="1a184-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a184-123">Type</span></span>|<span data-ttu-id="1a184-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a184-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a184-125">id</span><span class="sxs-lookup"><span data-stu-id="1a184-125">id</span></span>|<span data-ttu-id="1a184-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a184-126">String</span></span>|<span data-ttu-id="1a184-127">O identificador exclusivo no formato de tenantId_deviceId_requestId</span><span class="sxs-lookup"><span data-stu-id="1a184-127">The unique identifier in the form of tenantId_deviceId_requestId</span></span>|
|<span data-ttu-id="1a184-128">status</span><span class="sxs-lookup"><span data-stu-id="1a184-128">status</span></span>|<span data-ttu-id="1a184-129">String</span><span class="sxs-lookup"><span data-stu-id="1a184-129">String</span></span>|<span data-ttu-id="1a184-130">O status da solicitação de coleção de logs</span><span class="sxs-lookup"><span data-stu-id="1a184-130">The status of the log collection request</span></span>|
|<span data-ttu-id="1a184-131">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="1a184-131">managedDeviceId</span></span>|<span data-ttu-id="1a184-132">Guid</span><span class="sxs-lookup"><span data-stu-id="1a184-132">Guid</span></span>|<span data-ttu-id="1a184-133">A ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1a184-133">The device Id</span></span>|
|<span data-ttu-id="1a184-134">errorCode</span><span class="sxs-lookup"><span data-stu-id="1a184-134">errorCode</span></span>|<span data-ttu-id="1a184-135">Int64</span><span class="sxs-lookup"><span data-stu-id="1a184-135">Int64</span></span>|<span data-ttu-id="1a184-136">O código de erro, se houver.</span><span class="sxs-lookup"><span data-stu-id="1a184-136">The error code, if any.</span></span> <span data-ttu-id="1a184-137">Valores válidos-9.22337203685478 E + 18 para 9.22337203685478 E + 18</span><span class="sxs-lookup"><span data-stu-id="1a184-137">Valid values -9.22337203685478E+18 to 9.22337203685478E+18</span></span>|
|<span data-ttu-id="1a184-138">requestedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="1a184-138">requestedDateTimeUTC</span></span>|<span data-ttu-id="1a184-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a184-139">DateTimeOffset</span></span>|<span data-ttu-id="1a184-140">O DateTime da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a184-140">The DateTime of the request</span></span>|
|<span data-ttu-id="1a184-141">receivedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="1a184-141">receivedDateTimeUTC</span></span>|<span data-ttu-id="1a184-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a184-142">DateTimeOffset</span></span>|<span data-ttu-id="1a184-143">O DateTime que a solicitação foi recebida</span><span class="sxs-lookup"><span data-stu-id="1a184-143">The DateTime the request was received</span></span>|
|<span data-ttu-id="1a184-144">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1a184-144">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="1a184-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a184-145">String</span></span>|<span data-ttu-id="1a184-146">O UPN para quem iniciou a solicitação</span><span class="sxs-lookup"><span data-stu-id="1a184-146">The UPN for who initiated the request</span></span>|
|<span data-ttu-id="1a184-147">expirationDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="1a184-147">expirationDateTimeUTC</span></span>|<span data-ttu-id="1a184-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a184-148">DateTimeOffset</span></span>|<span data-ttu-id="1a184-149">O DateTime do vencimento dos logs</span><span class="sxs-lookup"><span data-stu-id="1a184-149">The DateTime of the expiration of the logs</span></span>|
|<span data-ttu-id="1a184-150">size</span><span class="sxs-lookup"><span data-stu-id="1a184-150">size</span></span>|<span data-ttu-id="1a184-151">Duplo</span><span class="sxs-lookup"><span data-stu-id="1a184-151">Double</span></span>|<span data-ttu-id="1a184-152">O tamanho dos logs.</span><span class="sxs-lookup"><span data-stu-id="1a184-152">The size of the logs.</span></span> <span data-ttu-id="1a184-153">Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="1a184-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a184-154">Relações</span><span class="sxs-lookup"><span data-stu-id="1a184-154">Relationships</span></span>
<span data-ttu-id="1a184-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a184-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a184-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a184-156">JSON Representation</span></span>
<span data-ttu-id="1a184-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a184-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceLogCollectionResponse"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
  "id": "String (identifier)",
  "status": "String",
  "managedDeviceId": "Guid",
  "errorCode": 1024,
  "requestedDateTimeUTC": "String (timestamp)",
  "receivedDateTimeUTC": "String (timestamp)",
  "initiatedByUserPrincipalName": "String",
  "expirationDateTimeUTC": "String (timestamp)",
  "size": "4.2"
}
```



