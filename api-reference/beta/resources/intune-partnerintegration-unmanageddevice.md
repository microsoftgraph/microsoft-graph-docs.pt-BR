---
title: Tipo de recurso unmanagedDevice
description: Dispositivo não-manageado descoberto na rede.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0163fb0f3704bee86622574428954b3c3c9f805a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160082"
---
# <a name="unmanageddevice-resource-type"></a><span data-ttu-id="b0638-103">Tipo de recurso unmanagedDevice</span><span class="sxs-lookup"><span data-stu-id="b0638-103">unmanagedDevice resource type</span></span>

<span data-ttu-id="b0638-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0638-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0638-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0638-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0638-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0638-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0638-107">Dispositivo não-manageado descoberto na rede.</span><span class="sxs-lookup"><span data-stu-id="b0638-107">Unmanaged device discovered in the network.</span></span>

## <a name="properties"></a><span data-ttu-id="b0638-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0638-108">Properties</span></span>
|<span data-ttu-id="b0638-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0638-109">Property</span></span>|<span data-ttu-id="b0638-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0638-110">Type</span></span>|<span data-ttu-id="b0638-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0638-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0638-112">so</span><span class="sxs-lookup"><span data-stu-id="b0638-112">os</span></span>|<span data-ttu-id="b0638-113">String</span><span class="sxs-lookup"><span data-stu-id="b0638-113">String</span></span>|<span data-ttu-id="b0638-114">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="b0638-114">Operating system.</span></span>|
|<span data-ttu-id="b0638-115">osVersion</span><span class="sxs-lookup"><span data-stu-id="b0638-115">osVersion</span></span>|<span data-ttu-id="b0638-116">String</span><span class="sxs-lookup"><span data-stu-id="b0638-116">String</span></span>|<span data-ttu-id="b0638-117">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="b0638-117">Operating system version.</span></span>|
|<span data-ttu-id="b0638-118">ipAddress</span><span class="sxs-lookup"><span data-stu-id="b0638-118">ipAddress</span></span>|<span data-ttu-id="b0638-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0638-119">String</span></span>|<span data-ttu-id="b0638-120">Endereço IP.</span><span class="sxs-lookup"><span data-stu-id="b0638-120">IP address.</span></span>|
|<span data-ttu-id="b0638-121">deviceName</span><span class="sxs-lookup"><span data-stu-id="b0638-121">deviceName</span></span>|<span data-ttu-id="b0638-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0638-122">String</span></span>|<span data-ttu-id="b0638-123">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0638-123">Device name.</span></span>|
|<span data-ttu-id="b0638-124">macAddress</span><span class="sxs-lookup"><span data-stu-id="b0638-124">macAddress</span></span>|<span data-ttu-id="b0638-125">String</span><span class="sxs-lookup"><span data-stu-id="b0638-125">String</span></span>|<span data-ttu-id="b0638-126">Endereço MAC.</span><span class="sxs-lookup"><span data-stu-id="b0638-126">MAC address.</span></span>|
|<span data-ttu-id="b0638-127">domínio</span><span class="sxs-lookup"><span data-stu-id="b0638-127">domain</span></span>|<span data-ttu-id="b0638-128">String</span><span class="sxs-lookup"><span data-stu-id="b0638-128">String</span></span>|<span data-ttu-id="b0638-129">Domínio.</span><span class="sxs-lookup"><span data-stu-id="b0638-129">Domain.</span></span>|
|<span data-ttu-id="b0638-130">fabricante</span><span class="sxs-lookup"><span data-stu-id="b0638-130">manufacturer</span></span>|<span data-ttu-id="b0638-131">String</span><span class="sxs-lookup"><span data-stu-id="b0638-131">String</span></span>|<span data-ttu-id="b0638-132">Fabricante.</span><span class="sxs-lookup"><span data-stu-id="b0638-132">Manufacturer.</span></span>|
|<span data-ttu-id="b0638-133">modelo</span><span class="sxs-lookup"><span data-stu-id="b0638-133">model</span></span>|<span data-ttu-id="b0638-134">String</span><span class="sxs-lookup"><span data-stu-id="b0638-134">String</span></span>|<span data-ttu-id="b0638-135">Modelo.</span><span class="sxs-lookup"><span data-stu-id="b0638-135">Model.</span></span>|
|<span data-ttu-id="b0638-136">localização</span><span class="sxs-lookup"><span data-stu-id="b0638-136">location</span></span>|<span data-ttu-id="b0638-137">String</span><span class="sxs-lookup"><span data-stu-id="b0638-137">String</span></span>|<span data-ttu-id="b0638-138">Localização.</span><span class="sxs-lookup"><span data-stu-id="b0638-138">Location.</span></span>|
|<span data-ttu-id="b0638-139">lastLoggedOnUser</span><span class="sxs-lookup"><span data-stu-id="b0638-139">lastLoggedOnUser</span></span>|<span data-ttu-id="b0638-140">String</span><span class="sxs-lookup"><span data-stu-id="b0638-140">String</span></span>|<span data-ttu-id="b0638-141">Último usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="b0638-141">Last logged on user.</span></span>|
|<span data-ttu-id="b0638-142">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="b0638-142">lastSeenDateTime</span></span>|<span data-ttu-id="b0638-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0638-143">DateTimeOffset</span></span>|<span data-ttu-id="b0638-144">Data e hora vistas pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b0638-144">Last seen date and time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0638-145">Relações</span><span class="sxs-lookup"><span data-stu-id="b0638-145">Relationships</span></span>
<span data-ttu-id="b0638-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0638-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0638-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0638-147">JSON Representation</span></span>
<span data-ttu-id="b0638-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0638-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unmanagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unmanagedDevice",
  "os": "String",
  "osVersion": "String",
  "ipAddress": "String",
  "deviceName": "String",
  "macAddress": "String",
  "domain": "String",
  "manufacturer": "String",
  "model": "String",
  "location": "String",
  "lastLoggedOnUser": "String",
  "lastSeenDateTime": "String (timestamp)"
}
```




