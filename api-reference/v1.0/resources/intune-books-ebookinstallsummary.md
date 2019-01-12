---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a3d07dc2d1a1b7a117e001546cd5298765676bdd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986149"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="98231-103">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="98231-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="98231-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="98231-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98231-105">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98231-105">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="98231-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="98231-106">Methods</span></span>
|<span data-ttu-id="98231-107">Método</span><span class="sxs-lookup"><span data-stu-id="98231-107">Method</span></span>|<span data-ttu-id="98231-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="98231-108">Return Type</span></span>|<span data-ttu-id="98231-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="98231-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="98231-110">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="98231-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="98231-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="98231-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="98231-112">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="98231-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="98231-113">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="98231-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="98231-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="98231-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="98231-115">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="98231-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="98231-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98231-116">Properties</span></span>
|<span data-ttu-id="98231-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98231-117">Property</span></span>|<span data-ttu-id="98231-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="98231-118">Type</span></span>|<span data-ttu-id="98231-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="98231-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98231-120">id</span><span class="sxs-lookup"><span data-stu-id="98231-120">id</span></span>|<span data-ttu-id="98231-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98231-121">String</span></span>|<span data-ttu-id="98231-122">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="98231-122">Key of the entity.</span></span>|
|<span data-ttu-id="98231-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98231-123">installedDeviceCount</span></span>|<span data-ttu-id="98231-124">Int32</span><span class="sxs-lookup"><span data-stu-id="98231-124">Int32</span></span>|<span data-ttu-id="98231-125">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="98231-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="98231-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98231-126">failedDeviceCount</span></span>|<span data-ttu-id="98231-127">Int32</span><span class="sxs-lookup"><span data-stu-id="98231-127">Int32</span></span>|<span data-ttu-id="98231-128">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="98231-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="98231-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98231-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="98231-130">Int32</span><span class="sxs-lookup"><span data-stu-id="98231-130">Int32</span></span>|<span data-ttu-id="98231-131">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="98231-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="98231-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="98231-132">installedUserCount</span></span>|<span data-ttu-id="98231-133">Int32</span><span class="sxs-lookup"><span data-stu-id="98231-133">Int32</span></span>|<span data-ttu-id="98231-134">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="98231-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="98231-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="98231-135">failedUserCount</span></span>|<span data-ttu-id="98231-136">Int32</span><span class="sxs-lookup"><span data-stu-id="98231-136">Int32</span></span>|<span data-ttu-id="98231-137">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="98231-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="98231-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="98231-138">notInstalledUserCount</span></span>|<span data-ttu-id="98231-139">Int32</span><span class="sxs-lookup"><span data-stu-id="98231-139">Int32</span></span>|<span data-ttu-id="98231-140">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="98231-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98231-141">Relações</span><span class="sxs-lookup"><span data-stu-id="98231-141">Relationships</span></span>
<span data-ttu-id="98231-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="98231-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="98231-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98231-143">JSON Representation</span></span>
<span data-ttu-id="98231-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="98231-144">Here is a JSON representation of the resource.</span></span>
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



