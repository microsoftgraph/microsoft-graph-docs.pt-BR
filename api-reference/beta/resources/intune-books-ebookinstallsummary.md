---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4eec97cd82224af5e74577a8d9ed9f378534263a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804393"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="5ad3c-103">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5ad3c-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="5ad3c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ad3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ad3c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ad3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ad3c-106">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ad3c-106">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="5ad3c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5ad3c-107">Methods</span></span>
|<span data-ttu-id="5ad3c-108">Método</span><span class="sxs-lookup"><span data-stu-id="5ad3c-108">Method</span></span>|<span data-ttu-id="5ad3c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5ad3c-109">Return Type</span></span>|<span data-ttu-id="5ad3c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ad3c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5ad3c-111">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5ad3c-111">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="5ad3c-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5ad3c-112">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="5ad3c-113">Ler propriedades e relações do objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="5ad3c-113">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="5ad3c-114">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5ad3c-114">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="5ad3c-115">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5ad3c-115">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="5ad3c-116">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="5ad3c-116">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5ad3c-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ad3c-117">Properties</span></span>
|<span data-ttu-id="5ad3c-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ad3c-118">Property</span></span>|<span data-ttu-id="5ad3c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ad3c-119">Type</span></span>|<span data-ttu-id="5ad3c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ad3c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ad3c-121">id</span><span class="sxs-lookup"><span data-stu-id="5ad3c-121">id</span></span>|<span data-ttu-id="5ad3c-122">String</span><span class="sxs-lookup"><span data-stu-id="5ad3c-122">String</span></span>|<span data-ttu-id="5ad3c-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ad3c-123">Key of the entity.</span></span>|
|<span data-ttu-id="5ad3c-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ad3c-124">installedDeviceCount</span></span>|<span data-ttu-id="5ad3c-125">Int32</span><span class="sxs-lookup"><span data-stu-id="5ad3c-125">Int32</span></span>|<span data-ttu-id="5ad3c-126">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="5ad3c-126">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="5ad3c-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ad3c-127">failedDeviceCount</span></span>|<span data-ttu-id="5ad3c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="5ad3c-128">Int32</span></span>|<span data-ttu-id="5ad3c-129">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="5ad3c-129">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="5ad3c-130">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ad3c-130">notInstalledDeviceCount</span></span>|<span data-ttu-id="5ad3c-131">Int32</span><span class="sxs-lookup"><span data-stu-id="5ad3c-131">Int32</span></span>|<span data-ttu-id="5ad3c-132">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="5ad3c-132">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="5ad3c-133">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="5ad3c-133">installedUserCount</span></span>|<span data-ttu-id="5ad3c-134">Int32</span><span class="sxs-lookup"><span data-stu-id="5ad3c-134">Int32</span></span>|<span data-ttu-id="5ad3c-135">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="5ad3c-135">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="5ad3c-136">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="5ad3c-136">failedUserCount</span></span>|<span data-ttu-id="5ad3c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5ad3c-137">Int32</span></span>|<span data-ttu-id="5ad3c-138">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="5ad3c-138">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="5ad3c-139">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="5ad3c-139">notInstalledUserCount</span></span>|<span data-ttu-id="5ad3c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5ad3c-140">Int32</span></span>|<span data-ttu-id="5ad3c-141">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="5ad3c-141">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ad3c-142">Relações</span><span class="sxs-lookup"><span data-stu-id="5ad3c-142">Relationships</span></span>
<span data-ttu-id="5ad3c-143">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5ad3c-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ad3c-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ad3c-144">JSON Representation</span></span>
<span data-ttu-id="5ad3c-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ad3c-145">Here is a JSON representation of the resource.</span></span>
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





