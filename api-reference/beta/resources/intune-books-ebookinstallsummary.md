---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3d3a5d1ce5c05d0a8c20a79aea2fd3562ab2170c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915939"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="e333a-103">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e333a-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="e333a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e333a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e333a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e333a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e333a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e333a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e333a-107">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e333a-107">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="e333a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="e333a-108">Methods</span></span>
|<span data-ttu-id="e333a-109">Método</span><span class="sxs-lookup"><span data-stu-id="e333a-109">Method</span></span>|<span data-ttu-id="e333a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e333a-110">Return Type</span></span>|<span data-ttu-id="e333a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e333a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e333a-112">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e333a-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="e333a-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e333a-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="e333a-114">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="e333a-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="e333a-115">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e333a-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="e333a-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e333a-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="e333a-117">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="e333a-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e333a-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e333a-118">Properties</span></span>
|<span data-ttu-id="e333a-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e333a-119">Property</span></span>|<span data-ttu-id="e333a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e333a-120">Type</span></span>|<span data-ttu-id="e333a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e333a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e333a-122">id</span><span class="sxs-lookup"><span data-stu-id="e333a-122">id</span></span>|<span data-ttu-id="e333a-123">String</span><span class="sxs-lookup"><span data-stu-id="e333a-123">String</span></span>|<span data-ttu-id="e333a-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e333a-124">Key of the entity.</span></span>|
|<span data-ttu-id="e333a-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e333a-125">installedDeviceCount</span></span>|<span data-ttu-id="e333a-126">Int32</span><span class="sxs-lookup"><span data-stu-id="e333a-126">Int32</span></span>|<span data-ttu-id="e333a-127">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="e333a-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="e333a-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e333a-128">failedDeviceCount</span></span>|<span data-ttu-id="e333a-129">Int32</span><span class="sxs-lookup"><span data-stu-id="e333a-129">Int32</span></span>|<span data-ttu-id="e333a-130">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="e333a-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="e333a-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e333a-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="e333a-132">Int32</span><span class="sxs-lookup"><span data-stu-id="e333a-132">Int32</span></span>|<span data-ttu-id="e333a-133">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="e333a-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="e333a-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="e333a-134">installedUserCount</span></span>|<span data-ttu-id="e333a-135">Int32</span><span class="sxs-lookup"><span data-stu-id="e333a-135">Int32</span></span>|<span data-ttu-id="e333a-136">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="e333a-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="e333a-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="e333a-137">failedUserCount</span></span>|<span data-ttu-id="e333a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="e333a-138">Int32</span></span>|<span data-ttu-id="e333a-139">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="e333a-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="e333a-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="e333a-140">notInstalledUserCount</span></span>|<span data-ttu-id="e333a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e333a-141">Int32</span></span>|<span data-ttu-id="e333a-142">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="e333a-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e333a-143">Relações</span><span class="sxs-lookup"><span data-stu-id="e333a-143">Relationships</span></span>
<span data-ttu-id="e333a-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e333a-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e333a-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e333a-145">JSON Representation</span></span>
<span data-ttu-id="e333a-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e333a-146">Here is a JSON representation of the resource.</span></span>
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





