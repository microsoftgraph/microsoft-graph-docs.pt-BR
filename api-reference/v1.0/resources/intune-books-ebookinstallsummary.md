---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
author: tfitzmac
ms.openlocfilehash: 4f94c82a0d7cd234206586829981c62ba7d0a959
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344272"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="bcfc5-103">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="bcfc5-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="bcfc5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bcfc5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bcfc5-105">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bcfc5-105">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="bcfc5-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="bcfc5-106">Methods</span></span>
|<span data-ttu-id="bcfc5-107">Método</span><span class="sxs-lookup"><span data-stu-id="bcfc5-107">Method</span></span>|<span data-ttu-id="bcfc5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bcfc5-108">Return Type</span></span>|<span data-ttu-id="bcfc5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcfc5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bcfc5-110">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="bcfc5-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="bcfc5-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="bcfc5-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="bcfc5-112">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="bcfc5-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="bcfc5-113">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="bcfc5-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="bcfc5-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="bcfc5-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="bcfc5-115">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="bcfc5-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bcfc5-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bcfc5-116">Properties</span></span>
|<span data-ttu-id="bcfc5-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bcfc5-117">Property</span></span>|<span data-ttu-id="bcfc5-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcfc5-118">Type</span></span>|<span data-ttu-id="bcfc5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcfc5-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcfc5-120">id</span><span class="sxs-lookup"><span data-stu-id="bcfc5-120">id</span></span>|<span data-ttu-id="bcfc5-121">String</span><span class="sxs-lookup"><span data-stu-id="bcfc5-121">String</span></span>|<span data-ttu-id="bcfc5-122">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bcfc5-122">Key of the entity.</span></span>|
|<span data-ttu-id="bcfc5-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bcfc5-123">installedDeviceCount</span></span>|<span data-ttu-id="bcfc5-124">Int32</span><span class="sxs-lookup"><span data-stu-id="bcfc5-124">Int32</span></span>|<span data-ttu-id="bcfc5-125">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="bcfc5-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="bcfc5-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bcfc5-126">failedDeviceCount</span></span>|<span data-ttu-id="bcfc5-127">Int32</span><span class="sxs-lookup"><span data-stu-id="bcfc5-127">Int32</span></span>|<span data-ttu-id="bcfc5-128">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="bcfc5-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="bcfc5-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bcfc5-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="bcfc5-130">Int32</span><span class="sxs-lookup"><span data-stu-id="bcfc5-130">Int32</span></span>|<span data-ttu-id="bcfc5-131">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="bcfc5-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="bcfc5-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="bcfc5-132">installedUserCount</span></span>|<span data-ttu-id="bcfc5-133">Int32</span><span class="sxs-lookup"><span data-stu-id="bcfc5-133">Int32</span></span>|<span data-ttu-id="bcfc5-134">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="bcfc5-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="bcfc5-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="bcfc5-135">failedUserCount</span></span>|<span data-ttu-id="bcfc5-136">Int32</span><span class="sxs-lookup"><span data-stu-id="bcfc5-136">Int32</span></span>|<span data-ttu-id="bcfc5-137">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="bcfc5-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="bcfc5-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="bcfc5-138">notInstalledUserCount</span></span>|<span data-ttu-id="bcfc5-139">Int32</span><span class="sxs-lookup"><span data-stu-id="bcfc5-139">Int32</span></span>|<span data-ttu-id="bcfc5-140">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="bcfc5-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bcfc5-141">Relações</span><span class="sxs-lookup"><span data-stu-id="bcfc5-141">Relationships</span></span>
<span data-ttu-id="bcfc5-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bcfc5-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bcfc5-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bcfc5-143">JSON Representation</span></span>
<span data-ttu-id="bcfc5-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bcfc5-144">Here is a JSON representation of the resource.</span></span>
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



