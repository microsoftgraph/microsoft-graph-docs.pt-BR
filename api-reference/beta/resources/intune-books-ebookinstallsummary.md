---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 48c973d32e401dd378ca06db0c11f57e6c07654f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42489164"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="a12f4-103">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="a12f4-103">eBookInstallSummary resource type</span></span>

<span data-ttu-id="a12f4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a12f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a12f4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a12f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a12f4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a12f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a12f4-107">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a12f4-107">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="a12f4-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="a12f4-108">Methods</span></span>
|<span data-ttu-id="a12f4-109">Método</span><span class="sxs-lookup"><span data-stu-id="a12f4-109">Method</span></span>|<span data-ttu-id="a12f4-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a12f4-110">Return Type</span></span>|<span data-ttu-id="a12f4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a12f4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a12f4-112">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="a12f4-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="a12f4-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="a12f4-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="a12f4-114">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a12f4-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="a12f4-115">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="a12f4-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="a12f4-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="a12f4-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="a12f4-117">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a12f4-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a12f4-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a12f4-118">Properties</span></span>
|<span data-ttu-id="a12f4-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a12f4-119">Property</span></span>|<span data-ttu-id="a12f4-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a12f4-120">Type</span></span>|<span data-ttu-id="a12f4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a12f4-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a12f4-122">id</span><span class="sxs-lookup"><span data-stu-id="a12f4-122">id</span></span>|<span data-ttu-id="a12f4-123">String</span><span class="sxs-lookup"><span data-stu-id="a12f4-123">String</span></span>|<span data-ttu-id="a12f4-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a12f4-124">Key of the entity.</span></span>|
|<span data-ttu-id="a12f4-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a12f4-125">installedDeviceCount</span></span>|<span data-ttu-id="a12f4-126">Int32</span><span class="sxs-lookup"><span data-stu-id="a12f4-126">Int32</span></span>|<span data-ttu-id="a12f4-127">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="a12f4-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="a12f4-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a12f4-128">failedDeviceCount</span></span>|<span data-ttu-id="a12f4-129">Int32</span><span class="sxs-lookup"><span data-stu-id="a12f4-129">Int32</span></span>|<span data-ttu-id="a12f4-130">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="a12f4-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="a12f4-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a12f4-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="a12f4-132">Int32</span><span class="sxs-lookup"><span data-stu-id="a12f4-132">Int32</span></span>|<span data-ttu-id="a12f4-133">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="a12f4-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="a12f4-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="a12f4-134">installedUserCount</span></span>|<span data-ttu-id="a12f4-135">Int32</span><span class="sxs-lookup"><span data-stu-id="a12f4-135">Int32</span></span>|<span data-ttu-id="a12f4-136">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="a12f4-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="a12f4-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="a12f4-137">failedUserCount</span></span>|<span data-ttu-id="a12f4-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a12f4-138">Int32</span></span>|<span data-ttu-id="a12f4-139">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="a12f4-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="a12f4-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="a12f4-140">notInstalledUserCount</span></span>|<span data-ttu-id="a12f4-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a12f4-141">Int32</span></span>|<span data-ttu-id="a12f4-142">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="a12f4-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a12f4-143">Relações</span><span class="sxs-lookup"><span data-stu-id="a12f4-143">Relationships</span></span>
<span data-ttu-id="a12f4-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a12f4-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a12f4-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a12f4-145">JSON Representation</span></span>
<span data-ttu-id="a12f4-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a12f4-146">Here is a JSON representation of the resource.</span></span>
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



