---
title: tipo de recurso de userAppInstallStatus
description: Contém propriedades para o status de instalação de um usuário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f17a504537b1230de175e033779441627f5f98be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938010"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="2ed7e-103">tipo de recurso de userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="2ed7e-103">userAppInstallStatus resource type</span></span>

> <span data-ttu-id="2ed7e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2ed7e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ed7e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2ed7e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ed7e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2ed7e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ed7e-107">Contém propriedades para o status de instalação de um usuário.</span><span class="sxs-lookup"><span data-stu-id="2ed7e-107">Contains properties for the installation status for a user.</span></span>
## <a name="methods"></a><span data-ttu-id="2ed7e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="2ed7e-108">Methods</span></span>
|<span data-ttu-id="2ed7e-109">Método</span><span class="sxs-lookup"><span data-stu-id="2ed7e-109">Method</span></span>|<span data-ttu-id="2ed7e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2ed7e-110">Return Type</span></span>|<span data-ttu-id="2ed7e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ed7e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ed7e-112">Lista userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="2ed7e-112">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="2ed7e-113">coleção [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="2ed7e-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="2ed7e-114">Lista as propriedades e os relacionamentos dos objetos [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="2ed7e-114">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="2ed7e-115">Obter userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="2ed7e-115">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="2ed7e-116">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="2ed7e-116">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="2ed7e-117">Leia as propriedades e os relacionamentos do objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="2ed7e-117">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="2ed7e-118">Criar userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="2ed7e-118">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="2ed7e-119">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="2ed7e-119">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="2ed7e-120">Crie um novo objeto de [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="2ed7e-120">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="2ed7e-121">Excluir userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="2ed7e-121">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="2ed7e-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ed7e-122">None</span></span>|<span data-ttu-id="2ed7e-123">Exclui um [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="2ed7e-123">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="2ed7e-124">Atualizar userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="2ed7e-124">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="2ed7e-125">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="2ed7e-125">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="2ed7e-126">Atualize as propriedades de um objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="2ed7e-126">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2ed7e-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ed7e-127">Properties</span></span>
|<span data-ttu-id="2ed7e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ed7e-128">Property</span></span>|<span data-ttu-id="2ed7e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ed7e-129">Type</span></span>|<span data-ttu-id="2ed7e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ed7e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ed7e-131">id</span><span class="sxs-lookup"><span data-stu-id="2ed7e-131">id</span></span>|<span data-ttu-id="2ed7e-132">String</span><span class="sxs-lookup"><span data-stu-id="2ed7e-132">String</span></span>|<span data-ttu-id="2ed7e-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2ed7e-133">Key of the entity.</span></span>|
|<span data-ttu-id="2ed7e-134">userName</span><span class="sxs-lookup"><span data-stu-id="2ed7e-134">userName</span></span>|<span data-ttu-id="2ed7e-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ed7e-135">String</span></span>|<span data-ttu-id="2ed7e-136">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="2ed7e-136">User name.</span></span>|
|<span data-ttu-id="2ed7e-137">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2ed7e-137">userPrincipalName</span></span>|<span data-ttu-id="2ed7e-138">String</span><span class="sxs-lookup"><span data-stu-id="2ed7e-138">String</span></span>|<span data-ttu-id="2ed7e-139">Nome Principal de usuário.</span><span class="sxs-lookup"><span data-stu-id="2ed7e-139">User Principal Name.</span></span>|
|<span data-ttu-id="2ed7e-140">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ed7e-140">installedDeviceCount</span></span>|<span data-ttu-id="2ed7e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="2ed7e-141">Int32</span></span>|<span data-ttu-id="2ed7e-142">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="2ed7e-142">Installed Device Count.</span></span>|
|<span data-ttu-id="2ed7e-143">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ed7e-143">failedDeviceCount</span></span>|<span data-ttu-id="2ed7e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="2ed7e-144">Int32</span></span>|<span data-ttu-id="2ed7e-145">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2ed7e-145">Failed Device Count.</span></span>|
|<span data-ttu-id="2ed7e-146">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ed7e-146">notInstalledDeviceCount</span></span>|<span data-ttu-id="2ed7e-147">Int32</span><span class="sxs-lookup"><span data-stu-id="2ed7e-147">Int32</span></span>|<span data-ttu-id="2ed7e-148">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="2ed7e-148">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ed7e-149">Relações</span><span class="sxs-lookup"><span data-stu-id="2ed7e-149">Relationships</span></span>
|<span data-ttu-id="2ed7e-150">Relação</span><span class="sxs-lookup"><span data-stu-id="2ed7e-150">Relationship</span></span>|<span data-ttu-id="2ed7e-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ed7e-151">Type</span></span>|<span data-ttu-id="2ed7e-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ed7e-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ed7e-153">app</span><span class="sxs-lookup"><span data-stu-id="2ed7e-153">app</span></span>|[<span data-ttu-id="2ed7e-154">mobileApp</span><span class="sxs-lookup"><span data-stu-id="2ed7e-154">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="2ed7e-155">O link de navegação para o aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="2ed7e-155">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="2ed7e-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="2ed7e-156">deviceStatuses</span></span>|<span data-ttu-id="2ed7e-157">coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="2ed7e-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="2ed7e-158">O estado de instalação do aplicativo em dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2ed7e-158">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ed7e-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ed7e-159">JSON Representation</span></span>
<span data-ttu-id="2ed7e-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ed7e-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "String (identifier)",
  "userName": "String",
  "userPrincipalName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```





