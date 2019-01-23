---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4e8952012624a038f497fea3c6b81ad364448a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415338"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="f3fda-103">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f3fda-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="f3fda-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f3fda-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f3fda-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f3fda-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3fda-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f3fda-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3fda-107">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3fda-107">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="f3fda-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="f3fda-108">Methods</span></span>
|<span data-ttu-id="f3fda-109">Método</span><span class="sxs-lookup"><span data-stu-id="f3fda-109">Method</span></span>|<span data-ttu-id="f3fda-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f3fda-110">Return Type</span></span>|<span data-ttu-id="f3fda-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3fda-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f3fda-112">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f3fda-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="f3fda-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f3fda-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="f3fda-114">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f3fda-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="f3fda-115">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f3fda-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="f3fda-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f3fda-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="f3fda-117">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f3fda-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3fda-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3fda-118">Properties</span></span>
|<span data-ttu-id="f3fda-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3fda-119">Property</span></span>|<span data-ttu-id="f3fda-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3fda-120">Type</span></span>|<span data-ttu-id="f3fda-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3fda-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3fda-122">id</span><span class="sxs-lookup"><span data-stu-id="f3fda-122">id</span></span>|<span data-ttu-id="f3fda-123">String</span><span class="sxs-lookup"><span data-stu-id="f3fda-123">String</span></span>|<span data-ttu-id="f3fda-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f3fda-124">Key of the entity.</span></span>|
|<span data-ttu-id="f3fda-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f3fda-125">installedDeviceCount</span></span>|<span data-ttu-id="f3fda-126">Int32</span><span class="sxs-lookup"><span data-stu-id="f3fda-126">Int32</span></span>|<span data-ttu-id="f3fda-127">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="f3fda-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="f3fda-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f3fda-128">failedDeviceCount</span></span>|<span data-ttu-id="f3fda-129">Int32</span><span class="sxs-lookup"><span data-stu-id="f3fda-129">Int32</span></span>|<span data-ttu-id="f3fda-130">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="f3fda-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="f3fda-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f3fda-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="f3fda-132">Int32</span><span class="sxs-lookup"><span data-stu-id="f3fda-132">Int32</span></span>|<span data-ttu-id="f3fda-133">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="f3fda-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="f3fda-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="f3fda-134">installedUserCount</span></span>|<span data-ttu-id="f3fda-135">Int32</span><span class="sxs-lookup"><span data-stu-id="f3fda-135">Int32</span></span>|<span data-ttu-id="f3fda-136">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="f3fda-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="f3fda-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="f3fda-137">failedUserCount</span></span>|<span data-ttu-id="f3fda-138">Int32</span><span class="sxs-lookup"><span data-stu-id="f3fda-138">Int32</span></span>|<span data-ttu-id="f3fda-139">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="f3fda-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="f3fda-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="f3fda-140">notInstalledUserCount</span></span>|<span data-ttu-id="f3fda-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f3fda-141">Int32</span></span>|<span data-ttu-id="f3fda-142">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="f3fda-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3fda-143">Relações</span><span class="sxs-lookup"><span data-stu-id="f3fda-143">Relationships</span></span>
<span data-ttu-id="f3fda-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f3fda-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3fda-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3fda-145">JSON Representation</span></span>
<span data-ttu-id="f3fda-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3fda-146">Here is a JSON representation of the resource.</span></span>
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




