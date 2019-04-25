---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17075183e0541669923a69c140d228cb1cbd4a2e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523914"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="cfc98-103">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="cfc98-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="cfc98-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cfc98-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfc98-105">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cfc98-105">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="cfc98-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="cfc98-106">Methods</span></span>
|<span data-ttu-id="cfc98-107">Método</span><span class="sxs-lookup"><span data-stu-id="cfc98-107">Method</span></span>|<span data-ttu-id="cfc98-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cfc98-108">Return Type</span></span>|<span data-ttu-id="cfc98-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfc98-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cfc98-110">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="cfc98-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="cfc98-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="cfc98-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="cfc98-112">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="cfc98-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="cfc98-113">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="cfc98-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="cfc98-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="cfc98-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="cfc98-115">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="cfc98-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cfc98-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cfc98-116">Properties</span></span>
|<span data-ttu-id="cfc98-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfc98-117">Property</span></span>|<span data-ttu-id="cfc98-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfc98-118">Type</span></span>|<span data-ttu-id="cfc98-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfc98-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfc98-120">id</span><span class="sxs-lookup"><span data-stu-id="cfc98-120">id</span></span>|<span data-ttu-id="cfc98-121">String</span><span class="sxs-lookup"><span data-stu-id="cfc98-121">String</span></span>|<span data-ttu-id="cfc98-122">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cfc98-122">Key of the entity.</span></span>|
|<span data-ttu-id="cfc98-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cfc98-123">installedDeviceCount</span></span>|<span data-ttu-id="cfc98-124">Int32</span><span class="sxs-lookup"><span data-stu-id="cfc98-124">Int32</span></span>|<span data-ttu-id="cfc98-125">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="cfc98-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="cfc98-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cfc98-126">failedDeviceCount</span></span>|<span data-ttu-id="cfc98-127">Int32</span><span class="sxs-lookup"><span data-stu-id="cfc98-127">Int32</span></span>|<span data-ttu-id="cfc98-128">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="cfc98-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="cfc98-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cfc98-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="cfc98-130">Int32</span><span class="sxs-lookup"><span data-stu-id="cfc98-130">Int32</span></span>|<span data-ttu-id="cfc98-131">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="cfc98-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="cfc98-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="cfc98-132">installedUserCount</span></span>|<span data-ttu-id="cfc98-133">Int32</span><span class="sxs-lookup"><span data-stu-id="cfc98-133">Int32</span></span>|<span data-ttu-id="cfc98-134">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="cfc98-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="cfc98-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="cfc98-135">failedUserCount</span></span>|<span data-ttu-id="cfc98-136">Int32</span><span class="sxs-lookup"><span data-stu-id="cfc98-136">Int32</span></span>|<span data-ttu-id="cfc98-137">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="cfc98-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="cfc98-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="cfc98-138">notInstalledUserCount</span></span>|<span data-ttu-id="cfc98-139">Int32</span><span class="sxs-lookup"><span data-stu-id="cfc98-139">Int32</span></span>|<span data-ttu-id="cfc98-140">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="cfc98-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfc98-141">Relações</span><span class="sxs-lookup"><span data-stu-id="cfc98-141">Relationships</span></span>
<span data-ttu-id="cfc98-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cfc98-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfc98-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cfc98-143">JSON Representation</span></span>
<span data-ttu-id="cfc98-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cfc98-144">Here is a JSON representation of the resource.</span></span>
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



