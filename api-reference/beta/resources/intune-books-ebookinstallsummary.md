---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f4132bf41a3081bc9b5234cfcd0066508baf1dee
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295408"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="c16a6-103">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="c16a6-103">eBookInstallSummary resource type</span></span>

<span data-ttu-id="c16a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c16a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c16a6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c16a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c16a6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c16a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c16a6-107">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c16a6-107">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="c16a6-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c16a6-108">Methods</span></span>
|<span data-ttu-id="c16a6-109">Método</span><span class="sxs-lookup"><span data-stu-id="c16a6-109">Method</span></span>|<span data-ttu-id="c16a6-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c16a6-110">Return Type</span></span>|<span data-ttu-id="c16a6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c16a6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c16a6-112">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="c16a6-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="c16a6-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="c16a6-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="c16a6-114">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c16a6-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="c16a6-115">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="c16a6-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="c16a6-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="c16a6-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="c16a6-117">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c16a6-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c16a6-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c16a6-118">Properties</span></span>
|<span data-ttu-id="c16a6-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c16a6-119">Property</span></span>|<span data-ttu-id="c16a6-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c16a6-120">Type</span></span>|<span data-ttu-id="c16a6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c16a6-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c16a6-122">id</span><span class="sxs-lookup"><span data-stu-id="c16a6-122">id</span></span>|<span data-ttu-id="c16a6-123">String</span><span class="sxs-lookup"><span data-stu-id="c16a6-123">String</span></span>|<span data-ttu-id="c16a6-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c16a6-124">Key of the entity.</span></span>|
|<span data-ttu-id="c16a6-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c16a6-125">installedDeviceCount</span></span>|<span data-ttu-id="c16a6-126">Int32</span><span class="sxs-lookup"><span data-stu-id="c16a6-126">Int32</span></span>|<span data-ttu-id="c16a6-127">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="c16a6-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="c16a6-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c16a6-128">failedDeviceCount</span></span>|<span data-ttu-id="c16a6-129">Int32</span><span class="sxs-lookup"><span data-stu-id="c16a6-129">Int32</span></span>|<span data-ttu-id="c16a6-130">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="c16a6-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="c16a6-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c16a6-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="c16a6-132">Int32</span><span class="sxs-lookup"><span data-stu-id="c16a6-132">Int32</span></span>|<span data-ttu-id="c16a6-133">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="c16a6-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="c16a6-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="c16a6-134">installedUserCount</span></span>|<span data-ttu-id="c16a6-135">Int32</span><span class="sxs-lookup"><span data-stu-id="c16a6-135">Int32</span></span>|<span data-ttu-id="c16a6-136">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="c16a6-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="c16a6-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="c16a6-137">failedUserCount</span></span>|<span data-ttu-id="c16a6-138">Int32</span><span class="sxs-lookup"><span data-stu-id="c16a6-138">Int32</span></span>|<span data-ttu-id="c16a6-139">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="c16a6-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="c16a6-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="c16a6-140">notInstalledUserCount</span></span>|<span data-ttu-id="c16a6-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c16a6-141">Int32</span></span>|<span data-ttu-id="c16a6-142">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="c16a6-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c16a6-143">Relações</span><span class="sxs-lookup"><span data-stu-id="c16a6-143">Relationships</span></span>
<span data-ttu-id="c16a6-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c16a6-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c16a6-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c16a6-145">JSON Representation</span></span>
<span data-ttu-id="c16a6-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c16a6-146">Here is a JSON representation of the resource.</span></span>
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




