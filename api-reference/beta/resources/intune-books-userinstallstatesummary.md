---
title: Tipo de recurso userInstallStateSummary
description: Contém as propriedades do resumo de estado de instalação de um usuário.
author: tfitzmac
ms.openlocfilehash: 3d8976cd7db7baabaec60bdf3fe2ed18094156c1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314382"
---
# <a name="userinstallstatesummary-resource-type"></a><span data-ttu-id="5fb70-103">Tipo de recurso userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="5fb70-103">userInstallStateSummary resource type</span></span>

> <span data-ttu-id="5fb70-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5fb70-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5fb70-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5fb70-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5fb70-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5fb70-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5fb70-107">Contém as propriedades do resumo de estado de instalação de um usuário.</span><span class="sxs-lookup"><span data-stu-id="5fb70-107">Contains properties for the installation state summary for a user.</span></span>
## <a name="methods"></a><span data-ttu-id="5fb70-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="5fb70-108">Methods</span></span>
|<span data-ttu-id="5fb70-109">Método</span><span class="sxs-lookup"><span data-stu-id="5fb70-109">Method</span></span>|<span data-ttu-id="5fb70-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5fb70-110">Return Type</span></span>|<span data-ttu-id="5fb70-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fb70-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5fb70-112">Listar userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="5fb70-112">List userInstallStateSummaries</span></span>](../api/intune-books-userinstallstatesummary-list.md)|<span data-ttu-id="5fb70-113">Conjunto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="5fb70-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="5fb70-114">Listar propriedades e relações de objetos de [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="5fb70-114">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="5fb70-115">Obter userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="5fb70-115">Get userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-get.md)|[<span data-ttu-id="5fb70-116">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="5fb70-116">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="5fb70-117">Ler propriedades e relações de objetos de [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="5fb70-117">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="5fb70-118">Criar userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="5fb70-118">Create userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-create.md)|[<span data-ttu-id="5fb70-119">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="5fb70-119">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="5fb70-120">Criar um novo objeto de [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="5fb70-120">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="5fb70-121">Excluir userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="5fb70-121">Delete userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-delete.md)|<span data-ttu-id="5fb70-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5fb70-122">None</span></span>|<span data-ttu-id="5fb70-123">Excluir [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="5fb70-123">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>|
|[<span data-ttu-id="5fb70-124">Atualizar userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="5fb70-124">Update userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-update.md)|[<span data-ttu-id="5fb70-125">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="5fb70-125">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="5fb70-126">Atualizar as propriedades de um objeto de [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="5fb70-126">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5fb70-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5fb70-127">Properties</span></span>
|<span data-ttu-id="5fb70-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5fb70-128">Property</span></span>|<span data-ttu-id="5fb70-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fb70-129">Type</span></span>|<span data-ttu-id="5fb70-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fb70-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fb70-131">id</span><span class="sxs-lookup"><span data-stu-id="5fb70-131">id</span></span>|<span data-ttu-id="5fb70-132">String</span><span class="sxs-lookup"><span data-stu-id="5fb70-132">String</span></span>|<span data-ttu-id="5fb70-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5fb70-133">Key of the entity.</span></span>|
|<span data-ttu-id="5fb70-134">userName</span><span class="sxs-lookup"><span data-stu-id="5fb70-134">userName</span></span>|<span data-ttu-id="5fb70-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5fb70-135">String</span></span>|<span data-ttu-id="5fb70-136">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="5fb70-136">User name.</span></span>|
|<span data-ttu-id="5fb70-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5fb70-137">installedDeviceCount</span></span>|<span data-ttu-id="5fb70-138">Int32</span><span class="sxs-lookup"><span data-stu-id="5fb70-138">Int32</span></span>|<span data-ttu-id="5fb70-139">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="5fb70-139">Installed Device Count.</span></span>|
|<span data-ttu-id="5fb70-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5fb70-140">failedDeviceCount</span></span>|<span data-ttu-id="5fb70-141">Int32</span><span class="sxs-lookup"><span data-stu-id="5fb70-141">Int32</span></span>|<span data-ttu-id="5fb70-142">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="5fb70-142">Failed Device Count.</span></span>|
|<span data-ttu-id="5fb70-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5fb70-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="5fb70-144">Int32</span><span class="sxs-lookup"><span data-stu-id="5fb70-144">Int32</span></span>|<span data-ttu-id="5fb70-145">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="5fb70-145">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fb70-146">Relações</span><span class="sxs-lookup"><span data-stu-id="5fb70-146">Relationships</span></span>
|<span data-ttu-id="5fb70-147">Relação</span><span class="sxs-lookup"><span data-stu-id="5fb70-147">Relationship</span></span>|<span data-ttu-id="5fb70-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fb70-148">Type</span></span>|<span data-ttu-id="5fb70-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fb70-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fb70-150">deviceStates</span><span class="sxs-lookup"><span data-stu-id="5fb70-150">deviceStates</span></span>|<span data-ttu-id="5fb70-151">Conjunto [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="5fb70-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="5fb70-152">O estado de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="5fb70-152">The install state of the eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5fb70-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5fb70-153">JSON Representation</span></span>
<span data-ttu-id="5fb70-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5fb70-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userInstallStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "String (identifier)",
  "userName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```





