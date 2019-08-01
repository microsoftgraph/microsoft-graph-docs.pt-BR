---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 82bc37303f815e782c3d2aac8e0c1b13eb8e6ec0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028844"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="ceae1-103">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ceae1-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="ceae1-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ceae1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ceae1-105">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ceae1-105">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="ceae1-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ceae1-106">Methods</span></span>
|<span data-ttu-id="ceae1-107">Método</span><span class="sxs-lookup"><span data-stu-id="ceae1-107">Method</span></span>|<span data-ttu-id="ceae1-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ceae1-108">Return Type</span></span>|<span data-ttu-id="ceae1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ceae1-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ceae1-110">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ceae1-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="ceae1-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ceae1-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="ceae1-112">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ceae1-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="ceae1-113">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ceae1-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="ceae1-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ceae1-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="ceae1-115">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ceae1-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ceae1-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ceae1-116">Properties</span></span>
|<span data-ttu-id="ceae1-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ceae1-117">Property</span></span>|<span data-ttu-id="ceae1-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="ceae1-118">Type</span></span>|<span data-ttu-id="ceae1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ceae1-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ceae1-120">id</span><span class="sxs-lookup"><span data-stu-id="ceae1-120">id</span></span>|<span data-ttu-id="ceae1-121">String</span><span class="sxs-lookup"><span data-stu-id="ceae1-121">String</span></span>|<span data-ttu-id="ceae1-122">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ceae1-122">Key of the entity.</span></span>|
|<span data-ttu-id="ceae1-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ceae1-123">installedDeviceCount</span></span>|<span data-ttu-id="ceae1-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ceae1-124">Int32</span></span>|<span data-ttu-id="ceae1-125">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="ceae1-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="ceae1-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ceae1-126">failedDeviceCount</span></span>|<span data-ttu-id="ceae1-127">Int32</span><span class="sxs-lookup"><span data-stu-id="ceae1-127">Int32</span></span>|<span data-ttu-id="ceae1-128">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="ceae1-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="ceae1-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ceae1-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="ceae1-130">Int32</span><span class="sxs-lookup"><span data-stu-id="ceae1-130">Int32</span></span>|<span data-ttu-id="ceae1-131">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="ceae1-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="ceae1-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="ceae1-132">installedUserCount</span></span>|<span data-ttu-id="ceae1-133">Int32</span><span class="sxs-lookup"><span data-stu-id="ceae1-133">Int32</span></span>|<span data-ttu-id="ceae1-134">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="ceae1-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="ceae1-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="ceae1-135">failedUserCount</span></span>|<span data-ttu-id="ceae1-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ceae1-136">Int32</span></span>|<span data-ttu-id="ceae1-137">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="ceae1-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="ceae1-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="ceae1-138">notInstalledUserCount</span></span>|<span data-ttu-id="ceae1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ceae1-139">Int32</span></span>|<span data-ttu-id="ceae1-140">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="ceae1-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ceae1-141">Relações</span><span class="sxs-lookup"><span data-stu-id="ceae1-141">Relationships</span></span>
<span data-ttu-id="ceae1-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ceae1-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ceae1-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ceae1-143">JSON Representation</span></span>
<span data-ttu-id="ceae1-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ceae1-144">Here is a JSON representation of the resource.</span></span>
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



