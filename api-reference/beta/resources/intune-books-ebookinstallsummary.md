---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1714b111399a1bf230bc208b0a1ebd4089a0cbd7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966608"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="caffd-103">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="caffd-103">eBookInstallSummary resource type</span></span>

<span data-ttu-id="caffd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="caffd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="caffd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="caffd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="caffd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="caffd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="caffd-107">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="caffd-107">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="caffd-108">Methods</span><span class="sxs-lookup"><span data-stu-id="caffd-108">Methods</span></span>
|<span data-ttu-id="caffd-109">Método</span><span class="sxs-lookup"><span data-stu-id="caffd-109">Method</span></span>|<span data-ttu-id="caffd-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="caffd-110">Return Type</span></span>|<span data-ttu-id="caffd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="caffd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="caffd-112">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="caffd-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="caffd-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="caffd-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="caffd-114">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="caffd-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="caffd-115">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="caffd-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="caffd-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="caffd-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="caffd-117">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="caffd-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="caffd-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="caffd-118">Properties</span></span>
|<span data-ttu-id="caffd-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="caffd-119">Property</span></span>|<span data-ttu-id="caffd-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="caffd-120">Type</span></span>|<span data-ttu-id="caffd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="caffd-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caffd-122">id</span><span class="sxs-lookup"><span data-stu-id="caffd-122">id</span></span>|<span data-ttu-id="caffd-123">String</span><span class="sxs-lookup"><span data-stu-id="caffd-123">String</span></span>|<span data-ttu-id="caffd-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="caffd-124">Key of the entity.</span></span>|
|<span data-ttu-id="caffd-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="caffd-125">installedDeviceCount</span></span>|<span data-ttu-id="caffd-126">Int32</span><span class="sxs-lookup"><span data-stu-id="caffd-126">Int32</span></span>|<span data-ttu-id="caffd-127">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="caffd-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="caffd-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="caffd-128">failedDeviceCount</span></span>|<span data-ttu-id="caffd-129">Int32</span><span class="sxs-lookup"><span data-stu-id="caffd-129">Int32</span></span>|<span data-ttu-id="caffd-130">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="caffd-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="caffd-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="caffd-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="caffd-132">Int32</span><span class="sxs-lookup"><span data-stu-id="caffd-132">Int32</span></span>|<span data-ttu-id="caffd-133">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="caffd-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="caffd-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="caffd-134">installedUserCount</span></span>|<span data-ttu-id="caffd-135">Int32</span><span class="sxs-lookup"><span data-stu-id="caffd-135">Int32</span></span>|<span data-ttu-id="caffd-136">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="caffd-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="caffd-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="caffd-137">failedUserCount</span></span>|<span data-ttu-id="caffd-138">Int32</span><span class="sxs-lookup"><span data-stu-id="caffd-138">Int32</span></span>|<span data-ttu-id="caffd-139">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="caffd-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="caffd-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="caffd-140">notInstalledUserCount</span></span>|<span data-ttu-id="caffd-141">Int32</span><span class="sxs-lookup"><span data-stu-id="caffd-141">Int32</span></span>|<span data-ttu-id="caffd-142">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="caffd-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="caffd-143">Relações</span><span class="sxs-lookup"><span data-stu-id="caffd-143">Relationships</span></span>
<span data-ttu-id="caffd-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="caffd-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="caffd-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="caffd-145">JSON Representation</span></span>
<span data-ttu-id="caffd-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="caffd-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```






