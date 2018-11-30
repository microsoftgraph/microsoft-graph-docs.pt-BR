---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
ms.openlocfilehash: 76ae1348572bc40d01c958f676983d09456dcf03
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036566"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="5e2b9-103">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5e2b9-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="5e2b9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5e2b9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e2b9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5e2b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e2b9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5e2b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e2b9-107">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e2b9-107">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="5e2b9-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="5e2b9-108">Methods</span></span>
|<span data-ttu-id="5e2b9-109">Método</span><span class="sxs-lookup"><span data-stu-id="5e2b9-109">Method</span></span>|<span data-ttu-id="5e2b9-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5e2b9-110">Return Type</span></span>|<span data-ttu-id="5e2b9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e2b9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5e2b9-112">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5e2b9-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="5e2b9-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5e2b9-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="5e2b9-114">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="5e2b9-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="5e2b9-115">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5e2b9-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="5e2b9-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5e2b9-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="5e2b9-117">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="5e2b9-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e2b9-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e2b9-118">Properties</span></span>
|<span data-ttu-id="5e2b9-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e2b9-119">Property</span></span>|<span data-ttu-id="5e2b9-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e2b9-120">Type</span></span>|<span data-ttu-id="5e2b9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e2b9-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e2b9-122">id</span><span class="sxs-lookup"><span data-stu-id="5e2b9-122">id</span></span>|<span data-ttu-id="5e2b9-123">String</span><span class="sxs-lookup"><span data-stu-id="5e2b9-123">String</span></span>|<span data-ttu-id="5e2b9-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5e2b9-124">Key of the entity.</span></span>|
|<span data-ttu-id="5e2b9-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5e2b9-125">installedDeviceCount</span></span>|<span data-ttu-id="5e2b9-126">Int32</span><span class="sxs-lookup"><span data-stu-id="5e2b9-126">Int32</span></span>|<span data-ttu-id="5e2b9-127">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="5e2b9-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="5e2b9-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5e2b9-128">failedDeviceCount</span></span>|<span data-ttu-id="5e2b9-129">Int32</span><span class="sxs-lookup"><span data-stu-id="5e2b9-129">Int32</span></span>|<span data-ttu-id="5e2b9-130">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="5e2b9-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="5e2b9-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5e2b9-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="5e2b9-132">Int32</span><span class="sxs-lookup"><span data-stu-id="5e2b9-132">Int32</span></span>|<span data-ttu-id="5e2b9-133">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="5e2b9-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="5e2b9-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="5e2b9-134">installedUserCount</span></span>|<span data-ttu-id="5e2b9-135">Int32</span><span class="sxs-lookup"><span data-stu-id="5e2b9-135">Int32</span></span>|<span data-ttu-id="5e2b9-136">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="5e2b9-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="5e2b9-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="5e2b9-137">failedUserCount</span></span>|<span data-ttu-id="5e2b9-138">Int32</span><span class="sxs-lookup"><span data-stu-id="5e2b9-138">Int32</span></span>|<span data-ttu-id="5e2b9-139">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="5e2b9-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="5e2b9-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="5e2b9-140">notInstalledUserCount</span></span>|<span data-ttu-id="5e2b9-141">Int32</span><span class="sxs-lookup"><span data-stu-id="5e2b9-141">Int32</span></span>|<span data-ttu-id="5e2b9-142">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="5e2b9-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e2b9-143">Relações</span><span class="sxs-lookup"><span data-stu-id="5e2b9-143">Relationships</span></span>
<span data-ttu-id="5e2b9-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e2b9-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5e2b9-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e2b9-145">JSON Representation</span></span>
<span data-ttu-id="5e2b9-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e2b9-146">Here is a JSON representation of the resource.</span></span>
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





