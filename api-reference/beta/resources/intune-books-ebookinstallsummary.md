---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e75b550f628958e0cfacd38c28bc61ca8c2430f0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706006"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="549b5-103">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="549b5-103">eBookInstallSummary resource type</span></span>

<span data-ttu-id="549b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="549b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="549b5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="549b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="549b5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="549b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="549b5-107">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="549b5-107">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="549b5-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="549b5-108">Methods</span></span>
|<span data-ttu-id="549b5-109">Método</span><span class="sxs-lookup"><span data-stu-id="549b5-109">Method</span></span>|<span data-ttu-id="549b5-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="549b5-110">Return Type</span></span>|<span data-ttu-id="549b5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="549b5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="549b5-112">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="549b5-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="549b5-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="549b5-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="549b5-114">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="549b5-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="549b5-115">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="549b5-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="549b5-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="549b5-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="549b5-117">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="549b5-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="549b5-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="549b5-118">Properties</span></span>
|<span data-ttu-id="549b5-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="549b5-119">Property</span></span>|<span data-ttu-id="549b5-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="549b5-120">Type</span></span>|<span data-ttu-id="549b5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="549b5-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="549b5-122">id</span><span class="sxs-lookup"><span data-stu-id="549b5-122">id</span></span>|<span data-ttu-id="549b5-123">String</span><span class="sxs-lookup"><span data-stu-id="549b5-123">String</span></span>|<span data-ttu-id="549b5-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="549b5-124">Key of the entity.</span></span>|
|<span data-ttu-id="549b5-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="549b5-125">installedDeviceCount</span></span>|<span data-ttu-id="549b5-126">Int32</span><span class="sxs-lookup"><span data-stu-id="549b5-126">Int32</span></span>|<span data-ttu-id="549b5-127">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="549b5-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="549b5-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="549b5-128">failedDeviceCount</span></span>|<span data-ttu-id="549b5-129">Int32</span><span class="sxs-lookup"><span data-stu-id="549b5-129">Int32</span></span>|<span data-ttu-id="549b5-130">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="549b5-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="549b5-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="549b5-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="549b5-132">Int32</span><span class="sxs-lookup"><span data-stu-id="549b5-132">Int32</span></span>|<span data-ttu-id="549b5-133">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="549b5-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="549b5-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="549b5-134">installedUserCount</span></span>|<span data-ttu-id="549b5-135">Int32</span><span class="sxs-lookup"><span data-stu-id="549b5-135">Int32</span></span>|<span data-ttu-id="549b5-136">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="549b5-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="549b5-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="549b5-137">failedUserCount</span></span>|<span data-ttu-id="549b5-138">Int32</span><span class="sxs-lookup"><span data-stu-id="549b5-138">Int32</span></span>|<span data-ttu-id="549b5-139">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="549b5-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="549b5-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="549b5-140">notInstalledUserCount</span></span>|<span data-ttu-id="549b5-141">Int32</span><span class="sxs-lookup"><span data-stu-id="549b5-141">Int32</span></span>|<span data-ttu-id="549b5-142">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="549b5-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="549b5-143">Relações</span><span class="sxs-lookup"><span data-stu-id="549b5-143">Relationships</span></span>
<span data-ttu-id="549b5-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="549b5-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="549b5-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="549b5-145">JSON Representation</span></span>
<span data-ttu-id="549b5-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="549b5-146">Here is a JSON representation of the resource.</span></span>
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





