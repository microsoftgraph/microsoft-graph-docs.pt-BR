---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b305d2814abf04725cd1a42acf05b90f96f0dd8b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472083"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="b55af-103">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b55af-103">eBookInstallSummary resource type</span></span>

<span data-ttu-id="b55af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b55af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b55af-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b55af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b55af-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b55af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b55af-107">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b55af-107">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="b55af-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b55af-108">Methods</span></span>
|<span data-ttu-id="b55af-109">Método</span><span class="sxs-lookup"><span data-stu-id="b55af-109">Method</span></span>|<span data-ttu-id="b55af-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b55af-110">Return Type</span></span>|<span data-ttu-id="b55af-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b55af-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b55af-112">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b55af-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="b55af-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b55af-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="b55af-114">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b55af-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="b55af-115">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b55af-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="b55af-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b55af-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="b55af-117">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b55af-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b55af-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b55af-118">Properties</span></span>
|<span data-ttu-id="b55af-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b55af-119">Property</span></span>|<span data-ttu-id="b55af-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b55af-120">Type</span></span>|<span data-ttu-id="b55af-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b55af-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b55af-122">id</span><span class="sxs-lookup"><span data-stu-id="b55af-122">id</span></span>|<span data-ttu-id="b55af-123">String</span><span class="sxs-lookup"><span data-stu-id="b55af-123">String</span></span>|<span data-ttu-id="b55af-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b55af-124">Key of the entity.</span></span>|
|<span data-ttu-id="b55af-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b55af-125">installedDeviceCount</span></span>|<span data-ttu-id="b55af-126">Int32</span><span class="sxs-lookup"><span data-stu-id="b55af-126">Int32</span></span>|<span data-ttu-id="b55af-127">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="b55af-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="b55af-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b55af-128">failedDeviceCount</span></span>|<span data-ttu-id="b55af-129">Int32</span><span class="sxs-lookup"><span data-stu-id="b55af-129">Int32</span></span>|<span data-ttu-id="b55af-130">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="b55af-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="b55af-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b55af-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="b55af-132">Int32</span><span class="sxs-lookup"><span data-stu-id="b55af-132">Int32</span></span>|<span data-ttu-id="b55af-133">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="b55af-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="b55af-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="b55af-134">installedUserCount</span></span>|<span data-ttu-id="b55af-135">Int32</span><span class="sxs-lookup"><span data-stu-id="b55af-135">Int32</span></span>|<span data-ttu-id="b55af-136">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="b55af-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="b55af-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="b55af-137">failedUserCount</span></span>|<span data-ttu-id="b55af-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b55af-138">Int32</span></span>|<span data-ttu-id="b55af-139">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="b55af-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="b55af-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="b55af-140">notInstalledUserCount</span></span>|<span data-ttu-id="b55af-141">Int32</span><span class="sxs-lookup"><span data-stu-id="b55af-141">Int32</span></span>|<span data-ttu-id="b55af-142">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="b55af-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b55af-143">Relações</span><span class="sxs-lookup"><span data-stu-id="b55af-143">Relationships</span></span>
<span data-ttu-id="b55af-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b55af-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b55af-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b55af-145">JSON Representation</span></span>
<span data-ttu-id="b55af-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b55af-146">Here is a JSON representation of the resource.</span></span>
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



