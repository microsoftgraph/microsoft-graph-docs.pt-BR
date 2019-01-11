---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b33f319106c39e11931726fcebcc8d5aa8d6ba46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825778"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="3c148-103">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3c148-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="3c148-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3c148-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c148-105">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3c148-105">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="3c148-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="3c148-106">Methods</span></span>
|<span data-ttu-id="3c148-107">Método</span><span class="sxs-lookup"><span data-stu-id="3c148-107">Method</span></span>|<span data-ttu-id="3c148-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3c148-108">Return Type</span></span>|<span data-ttu-id="3c148-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c148-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3c148-110">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3c148-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="3c148-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3c148-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="3c148-112">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="3c148-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="3c148-113">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3c148-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="3c148-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3c148-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="3c148-115">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="3c148-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3c148-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c148-116">Properties</span></span>
|<span data-ttu-id="3c148-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c148-117">Property</span></span>|<span data-ttu-id="3c148-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c148-118">Type</span></span>|<span data-ttu-id="3c148-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c148-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c148-120">id</span><span class="sxs-lookup"><span data-stu-id="3c148-120">id</span></span>|<span data-ttu-id="3c148-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c148-121">String</span></span>|<span data-ttu-id="3c148-122">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3c148-122">Key of the entity.</span></span>|
|<span data-ttu-id="3c148-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3c148-123">installedDeviceCount</span></span>|<span data-ttu-id="3c148-124">Int32</span><span class="sxs-lookup"><span data-stu-id="3c148-124">Int32</span></span>|<span data-ttu-id="3c148-125">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="3c148-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="3c148-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3c148-126">failedDeviceCount</span></span>|<span data-ttu-id="3c148-127">Int32</span><span class="sxs-lookup"><span data-stu-id="3c148-127">Int32</span></span>|<span data-ttu-id="3c148-128">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="3c148-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="3c148-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3c148-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="3c148-130">Int32</span><span class="sxs-lookup"><span data-stu-id="3c148-130">Int32</span></span>|<span data-ttu-id="3c148-131">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="3c148-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="3c148-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="3c148-132">installedUserCount</span></span>|<span data-ttu-id="3c148-133">Int32</span><span class="sxs-lookup"><span data-stu-id="3c148-133">Int32</span></span>|<span data-ttu-id="3c148-134">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="3c148-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="3c148-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="3c148-135">failedUserCount</span></span>|<span data-ttu-id="3c148-136">Int32</span><span class="sxs-lookup"><span data-stu-id="3c148-136">Int32</span></span>|<span data-ttu-id="3c148-137">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="3c148-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="3c148-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="3c148-138">notInstalledUserCount</span></span>|<span data-ttu-id="3c148-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3c148-139">Int32</span></span>|<span data-ttu-id="3c148-140">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="3c148-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c148-141">Relações</span><span class="sxs-lookup"><span data-stu-id="3c148-141">Relationships</span></span>
<span data-ttu-id="3c148-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c148-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3c148-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c148-143">JSON Representation</span></span>
<span data-ttu-id="3c148-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c148-144">Here is a JSON representation of the resource.</span></span>
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



