---
title: tipo de recurso de userAppInstallStatus
description: Contém propriedades para o status de instalação de um usuário.
author: tfitzmac
ms.openlocfilehash: 024fff32aac2a268a2e0bbec81a6d46b31012a11
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302755"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="10dd7-103">tipo de recurso de userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="10dd7-103">userAppInstallStatus resource type</span></span>

> <span data-ttu-id="10dd7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="10dd7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10dd7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="10dd7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10dd7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="10dd7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10dd7-107">Contém propriedades para o status de instalação de um usuário.</span><span class="sxs-lookup"><span data-stu-id="10dd7-107">Contains properties for the installation status for a user.</span></span>
## <a name="methods"></a><span data-ttu-id="10dd7-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="10dd7-108">Methods</span></span>
|<span data-ttu-id="10dd7-109">Método</span><span class="sxs-lookup"><span data-stu-id="10dd7-109">Method</span></span>|<span data-ttu-id="10dd7-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="10dd7-110">Return Type</span></span>|<span data-ttu-id="10dd7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="10dd7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="10dd7-112">Lista userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="10dd7-112">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="10dd7-113">coleção [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="10dd7-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="10dd7-114">Lista as propriedades e os relacionamentos dos objetos [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="10dd7-114">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="10dd7-115">Obter userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="10dd7-115">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="10dd7-116">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="10dd7-116">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="10dd7-117">Leia as propriedades e os relacionamentos do objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="10dd7-117">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="10dd7-118">Criar userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="10dd7-118">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="10dd7-119">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="10dd7-119">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="10dd7-120">Crie um novo objeto de [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="10dd7-120">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="10dd7-121">Excluir userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="10dd7-121">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="10dd7-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10dd7-122">None</span></span>|<span data-ttu-id="10dd7-123">Exclui um [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="10dd7-123">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="10dd7-124">Atualizar userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="10dd7-124">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="10dd7-125">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="10dd7-125">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="10dd7-126">Atualize as propriedades de um objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="10dd7-126">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="10dd7-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10dd7-127">Properties</span></span>
|<span data-ttu-id="10dd7-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10dd7-128">Property</span></span>|<span data-ttu-id="10dd7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="10dd7-129">Type</span></span>|<span data-ttu-id="10dd7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="10dd7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10dd7-131">id</span><span class="sxs-lookup"><span data-stu-id="10dd7-131">id</span></span>|<span data-ttu-id="10dd7-132">String</span><span class="sxs-lookup"><span data-stu-id="10dd7-132">String</span></span>|<span data-ttu-id="10dd7-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="10dd7-133">Key of the entity.</span></span>|
|<span data-ttu-id="10dd7-134">userName</span><span class="sxs-lookup"><span data-stu-id="10dd7-134">userName</span></span>|<span data-ttu-id="10dd7-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10dd7-135">String</span></span>|<span data-ttu-id="10dd7-136">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="10dd7-136">User name.</span></span>|
|<span data-ttu-id="10dd7-137">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="10dd7-137">userPrincipalName</span></span>|<span data-ttu-id="10dd7-138">String</span><span class="sxs-lookup"><span data-stu-id="10dd7-138">String</span></span>|<span data-ttu-id="10dd7-139">Nome Principal de usuário.</span><span class="sxs-lookup"><span data-stu-id="10dd7-139">User Principal Name.</span></span>|
|<span data-ttu-id="10dd7-140">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="10dd7-140">installedDeviceCount</span></span>|<span data-ttu-id="10dd7-141">Int32</span><span class="sxs-lookup"><span data-stu-id="10dd7-141">Int32</span></span>|<span data-ttu-id="10dd7-142">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="10dd7-142">Installed Device Count.</span></span>|
|<span data-ttu-id="10dd7-143">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="10dd7-143">failedDeviceCount</span></span>|<span data-ttu-id="10dd7-144">Int32</span><span class="sxs-lookup"><span data-stu-id="10dd7-144">Int32</span></span>|<span data-ttu-id="10dd7-145">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="10dd7-145">Failed Device Count.</span></span>|
|<span data-ttu-id="10dd7-146">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="10dd7-146">notInstalledDeviceCount</span></span>|<span data-ttu-id="10dd7-147">Int32</span><span class="sxs-lookup"><span data-stu-id="10dd7-147">Int32</span></span>|<span data-ttu-id="10dd7-148">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="10dd7-148">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10dd7-149">Relações</span><span class="sxs-lookup"><span data-stu-id="10dd7-149">Relationships</span></span>
|<span data-ttu-id="10dd7-150">Relação</span><span class="sxs-lookup"><span data-stu-id="10dd7-150">Relationship</span></span>|<span data-ttu-id="10dd7-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="10dd7-151">Type</span></span>|<span data-ttu-id="10dd7-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="10dd7-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10dd7-153">app</span><span class="sxs-lookup"><span data-stu-id="10dd7-153">app</span></span>|[<span data-ttu-id="10dd7-154">mobileApp</span><span class="sxs-lookup"><span data-stu-id="10dd7-154">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="10dd7-155">O link de navegação para o aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="10dd7-155">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="10dd7-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="10dd7-156">deviceStatuses</span></span>|<span data-ttu-id="10dd7-157">coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="10dd7-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="10dd7-158">O estado de instalação do aplicativo em dispositivos.</span><span class="sxs-lookup"><span data-stu-id="10dd7-158">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10dd7-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10dd7-159">JSON Representation</span></span>
<span data-ttu-id="10dd7-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10dd7-160">Here is a JSON representation of the resource.</span></span>
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





