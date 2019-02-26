---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17075183e0541669923a69c140d228cb1cbd4a2e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251535"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="73b33-103">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="73b33-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="73b33-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73b33-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73b33-105">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73b33-105">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="73b33-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="73b33-106">Methods</span></span>
|<span data-ttu-id="73b33-107">Método</span><span class="sxs-lookup"><span data-stu-id="73b33-107">Method</span></span>|<span data-ttu-id="73b33-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="73b33-108">Return Type</span></span>|<span data-ttu-id="73b33-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="73b33-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="73b33-110">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="73b33-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="73b33-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="73b33-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="73b33-112">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="73b33-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="73b33-113">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="73b33-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="73b33-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="73b33-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="73b33-115">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="73b33-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="73b33-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73b33-116">Properties</span></span>
|<span data-ttu-id="73b33-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73b33-117">Property</span></span>|<span data-ttu-id="73b33-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="73b33-118">Type</span></span>|<span data-ttu-id="73b33-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="73b33-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73b33-120">id</span><span class="sxs-lookup"><span data-stu-id="73b33-120">id</span></span>|<span data-ttu-id="73b33-121">String</span><span class="sxs-lookup"><span data-stu-id="73b33-121">String</span></span>|<span data-ttu-id="73b33-122">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="73b33-122">Key of the entity.</span></span>|
|<span data-ttu-id="73b33-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="73b33-123">installedDeviceCount</span></span>|<span data-ttu-id="73b33-124">Int32</span><span class="sxs-lookup"><span data-stu-id="73b33-124">Int32</span></span>|<span data-ttu-id="73b33-125">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="73b33-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="73b33-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="73b33-126">failedDeviceCount</span></span>|<span data-ttu-id="73b33-127">Int32</span><span class="sxs-lookup"><span data-stu-id="73b33-127">Int32</span></span>|<span data-ttu-id="73b33-128">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="73b33-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="73b33-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="73b33-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="73b33-130">Int32</span><span class="sxs-lookup"><span data-stu-id="73b33-130">Int32</span></span>|<span data-ttu-id="73b33-131">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="73b33-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="73b33-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="73b33-132">installedUserCount</span></span>|<span data-ttu-id="73b33-133">Int32</span><span class="sxs-lookup"><span data-stu-id="73b33-133">Int32</span></span>|<span data-ttu-id="73b33-134">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="73b33-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="73b33-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="73b33-135">failedUserCount</span></span>|<span data-ttu-id="73b33-136">Int32</span><span class="sxs-lookup"><span data-stu-id="73b33-136">Int32</span></span>|<span data-ttu-id="73b33-137">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="73b33-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="73b33-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="73b33-138">notInstalledUserCount</span></span>|<span data-ttu-id="73b33-139">Int32</span><span class="sxs-lookup"><span data-stu-id="73b33-139">Int32</span></span>|<span data-ttu-id="73b33-140">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="73b33-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73b33-141">Relações</span><span class="sxs-lookup"><span data-stu-id="73b33-141">Relationships</span></span>
<span data-ttu-id="73b33-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73b33-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73b33-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73b33-143">JSON Representation</span></span>
<span data-ttu-id="73b33-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73b33-144">Here is a JSON representation of the resource.</span></span>
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



