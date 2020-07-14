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
# <a name="devicelogcollectionresponse-resource-type"></a><span data-ttu-id="34770-103">tipo de recurso deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="34770-103">deviceLogCollectionResponse resource type</span></span>

<span data-ttu-id="34770-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34770-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34770-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34770-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34770-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34770-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34770-107">Entidade de solicitação de conjunto de logs do Windows.</span><span class="sxs-lookup"><span data-stu-id="34770-107">Windows Log Collection request entity.</span></span>

## <a name="methods"></a><span data-ttu-id="34770-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="34770-108">Methods</span></span>
|<span data-ttu-id="34770-109">Método</span><span class="sxs-lookup"><span data-stu-id="34770-109">Method</span></span>|<span data-ttu-id="34770-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="34770-110">Return Type</span></span>|<span data-ttu-id="34770-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="34770-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="34770-112">Listar deviceLogCollectionResponses</span><span class="sxs-lookup"><span data-stu-id="34770-112">List deviceLogCollectionResponses</span></span>](../api/intune-devices-devicelogcollectionresponse-list.md)|<span data-ttu-id="34770-113">coleção [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="34770-113">[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) collection</span></span>|<span data-ttu-id="34770-114">Listar Propriedades e relações dos objetos [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="34770-114">List properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) objects.</span></span>|
|[<span data-ttu-id="34770-115">Obter deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="34770-115">Get deviceLogCollectionResponse</span></span>](../api/intune-devices-devicelogcollectionresponse-get.md)|[<span data-ttu-id="34770-116">deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="34770-116">deviceLogCollectionResponse</span></span>](../resources/intune-devices-devicelogcollectionresponse.md)|<span data-ttu-id="34770-117">Leia as propriedades e as relações do objeto [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="34770-117">Read properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>|
|[<span data-ttu-id="34770-118">ação createDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="34770-118">createDownloadUrl action</span></span>](../api/intune-devices-devicelogcollectionresponse-createdownloadurl.md)|<span data-ttu-id="34770-119">String</span><span class="sxs-lookup"><span data-stu-id="34770-119">String</span></span>|<span data-ttu-id="34770-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="34770-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="34770-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34770-121">Properties</span></span>
|<span data-ttu-id="34770-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34770-122">Property</span></span>|<span data-ttu-id="34770-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="34770-123">Type</span></span>|<span data-ttu-id="34770-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="34770-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34770-125">id</span><span class="sxs-lookup"><span data-stu-id="34770-125">id</span></span>|<span data-ttu-id="34770-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34770-126">String</span></span>|<span data-ttu-id="34770-127">O identificador exclusivo no formato de tenantId_deviceId_requestId</span><span class="sxs-lookup"><span data-stu-id="34770-127">The unique identifier in the form of tenantId_deviceId_requestId</span></span>|
|<span data-ttu-id="34770-128">status</span><span class="sxs-lookup"><span data-stu-id="34770-128">status</span></span>|<span data-ttu-id="34770-129">String</span><span class="sxs-lookup"><span data-stu-id="34770-129">String</span></span>|<span data-ttu-id="34770-130">O status da solicitação de coleção de logs</span><span class="sxs-lookup"><span data-stu-id="34770-130">The status of the log collection request</span></span>|
|<span data-ttu-id="34770-131">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="34770-131">managedDeviceId</span></span>|<span data-ttu-id="34770-132">Guid</span><span class="sxs-lookup"><span data-stu-id="34770-132">Guid</span></span>|<span data-ttu-id="34770-133">A ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="34770-133">The device Id</span></span>|
|<span data-ttu-id="34770-134">errorCode</span><span class="sxs-lookup"><span data-stu-id="34770-134">errorCode</span></span>|<span data-ttu-id="34770-135">Int64</span><span class="sxs-lookup"><span data-stu-id="34770-135">Int64</span></span>|<span data-ttu-id="34770-136">O código de erro, se houver.</span><span class="sxs-lookup"><span data-stu-id="34770-136">The error code, if any.</span></span> <span data-ttu-id="34770-137">Valores válidos-9.22337203685478 E + 18 para 9.22337203685478 E + 18</span><span class="sxs-lookup"><span data-stu-id="34770-137">Valid values -9.22337203685478E+18 to 9.22337203685478E+18</span></span>|
|<span data-ttu-id="34770-138">requestedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="34770-138">requestedDateTimeUTC</span></span>|<span data-ttu-id="34770-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34770-139">DateTimeOffset</span></span>|<span data-ttu-id="34770-140">O DateTime da solicitação</span><span class="sxs-lookup"><span data-stu-id="34770-140">The DateTime of the request</span></span>|
|<span data-ttu-id="34770-141">receivedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="34770-141">receivedDateTimeUTC</span></span>|<span data-ttu-id="34770-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34770-142">DateTimeOffset</span></span>|<span data-ttu-id="34770-143">O DateTime que a solicitação foi recebida</span><span class="sxs-lookup"><span data-stu-id="34770-143">The DateTime the request was received</span></span>|
|<span data-ttu-id="34770-144">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="34770-144">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="34770-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34770-145">String</span></span>|<span data-ttu-id="34770-146">O UPN para quem iniciou a solicitação</span><span class="sxs-lookup"><span data-stu-id="34770-146">The UPN for who initiated the request</span></span>|
|<span data-ttu-id="34770-147">expirationDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="34770-147">expirationDateTimeUTC</span></span>|<span data-ttu-id="34770-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34770-148">DateTimeOffset</span></span>|<span data-ttu-id="34770-149">O DateTime do vencimento dos logs</span><span class="sxs-lookup"><span data-stu-id="34770-149">The DateTime of the expiration of the logs</span></span>|
|<span data-ttu-id="34770-150">size</span><span class="sxs-lookup"><span data-stu-id="34770-150">size</span></span>|<span data-ttu-id="34770-151">Duplo</span><span class="sxs-lookup"><span data-stu-id="34770-151">Double</span></span>|<span data-ttu-id="34770-152">O tamanho dos logs.</span><span class="sxs-lookup"><span data-stu-id="34770-152">The size of the logs.</span></span> <span data-ttu-id="34770-153">Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="34770-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|

## <a name="relationships"></a><span data-ttu-id="34770-154">Relações</span><span class="sxs-lookup"><span data-stu-id="34770-154">Relationships</span></span>
<span data-ttu-id="34770-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34770-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34770-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34770-156">JSON Representation</span></span>
<span data-ttu-id="34770-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34770-157">Here is a JSON representation of the resource.</span></span>
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



