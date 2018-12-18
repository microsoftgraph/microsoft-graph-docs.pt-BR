---
title: Tipo de recurso deviceInstallState
description: Contém propriedades do estado de instalação de um dispositivo.
author: tfitzmac
ms.openlocfilehash: fb11f93682093655a38ac554b2816348f9b0c6bc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360365"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="b8e99-103">Tipo de recurso deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="b8e99-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="b8e99-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b8e99-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8e99-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b8e99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8e99-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b8e99-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8e99-107">Contém propriedades do estado de instalação de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b8e99-107">Contains properties for the installation state for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="b8e99-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b8e99-108">Methods</span></span>
|<span data-ttu-id="b8e99-109">Método</span><span class="sxs-lookup"><span data-stu-id="b8e99-109">Method</span></span>|<span data-ttu-id="b8e99-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b8e99-110">Return Type</span></span>|<span data-ttu-id="b8e99-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8e99-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b8e99-112">Listar deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="b8e99-112">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="b8e99-113">Conjunto [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="b8e99-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="b8e99-114">Lê propriedades e relações de objetos de [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="b8e99-114">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="b8e99-115">Obter deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="b8e99-115">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="b8e99-116">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="b8e99-116">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="b8e99-117">Ler propriedades e relações de objetos de [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="b8e99-117">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="b8e99-118">Criar deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="b8e99-118">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="b8e99-119">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="b8e99-119">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="b8e99-120">Crie um novo objeto de [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="b8e99-120">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="b8e99-121">Excluir deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="b8e99-121">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="b8e99-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8e99-122">None</span></span>|<span data-ttu-id="b8e99-123">Excluir [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="b8e99-123">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="b8e99-124">Atualizar deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="b8e99-124">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="b8e99-125">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="b8e99-125">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="b8e99-126">Atualizar as propriedades de um objeto de [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="b8e99-126">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8e99-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8e99-127">Properties</span></span>
|<span data-ttu-id="b8e99-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8e99-128">Property</span></span>|<span data-ttu-id="b8e99-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8e99-129">Type</span></span>|<span data-ttu-id="b8e99-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8e99-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8e99-131">id</span><span class="sxs-lookup"><span data-stu-id="b8e99-131">id</span></span>|<span data-ttu-id="b8e99-132">String</span><span class="sxs-lookup"><span data-stu-id="b8e99-132">String</span></span>|<span data-ttu-id="b8e99-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b8e99-133">Key of the entity.</span></span>|
|<span data-ttu-id="b8e99-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="b8e99-134">deviceName</span></span>|<span data-ttu-id="b8e99-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8e99-135">String</span></span>|<span data-ttu-id="b8e99-136">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b8e99-136">Device name.</span></span>|
|<span data-ttu-id="b8e99-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="b8e99-137">deviceId</span></span>|<span data-ttu-id="b8e99-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8e99-138">String</span></span>|<span data-ttu-id="b8e99-139">ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b8e99-139">Device Id.</span></span>|
|<span data-ttu-id="b8e99-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b8e99-140">lastSyncDateTime</span></span>|<span data-ttu-id="b8e99-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8e99-141">DateTimeOffset</span></span>|<span data-ttu-id="b8e99-142">Última sincronização de data e hora.</span><span class="sxs-lookup"><span data-stu-id="b8e99-142">Last sync date and time.</span></span>|
|<span data-ttu-id="b8e99-143">installState</span><span class="sxs-lookup"><span data-stu-id="b8e99-143">installState</span></span>|[<span data-ttu-id="b8e99-144">installState</span><span class="sxs-lookup"><span data-stu-id="b8e99-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="b8e99-145">O estado de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="b8e99-145">The install state of the eBook.</span></span> <span data-ttu-id="b8e99-146">Os valores possíveis são: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b8e99-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="b8e99-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="b8e99-147">errorCode</span></span>|<span data-ttu-id="b8e99-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8e99-148">String</span></span>|<span data-ttu-id="b8e99-149">O código de erro de falhas de instalação.</span><span class="sxs-lookup"><span data-stu-id="b8e99-149">The error code for install failures.</span></span>|
|<span data-ttu-id="b8e99-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="b8e99-150">osVersion</span></span>|<span data-ttu-id="b8e99-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8e99-151">String</span></span>|<span data-ttu-id="b8e99-152">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="b8e99-152">OS Version.</span></span>|
|<span data-ttu-id="b8e99-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="b8e99-153">osDescription</span></span>|<span data-ttu-id="b8e99-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8e99-154">String</span></span>|<span data-ttu-id="b8e99-155">Descrição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="b8e99-155">OS Description.</span></span>|
|<span data-ttu-id="b8e99-156">userName</span><span class="sxs-lookup"><span data-stu-id="b8e99-156">userName</span></span>|<span data-ttu-id="b8e99-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8e99-157">String</span></span>|<span data-ttu-id="b8e99-158">Nome de usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b8e99-158">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8e99-159">Relações</span><span class="sxs-lookup"><span data-stu-id="b8e99-159">Relationships</span></span>
<span data-ttu-id="b8e99-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8e99-160">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8e99-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8e99-161">JSON Representation</span></span>
<span data-ttu-id="b8e99-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8e99-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```





