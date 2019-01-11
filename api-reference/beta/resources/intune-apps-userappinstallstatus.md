---
title: tipo de recurso de userAppInstallStatus
description: Contém propriedades para o status de instalação de um usuário.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f4d848a4fe4cd742df8a83184d539d7ff27290b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885201"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="6e459-103">tipo de recurso de userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6e459-103">userAppInstallStatus resource type</span></span>

> <span data-ttu-id="6e459-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6e459-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e459-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6e459-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e459-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6e459-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e459-107">Contém propriedades para o status de instalação de um usuário.</span><span class="sxs-lookup"><span data-stu-id="6e459-107">Contains properties for the installation status for a user.</span></span>
## <a name="methods"></a><span data-ttu-id="6e459-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="6e459-108">Methods</span></span>
|<span data-ttu-id="6e459-109">Método</span><span class="sxs-lookup"><span data-stu-id="6e459-109">Method</span></span>|<span data-ttu-id="6e459-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6e459-110">Return Type</span></span>|<span data-ttu-id="6e459-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e459-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6e459-112">Lista userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="6e459-112">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="6e459-113">coleção [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="6e459-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="6e459-114">Lista as propriedades e os relacionamentos dos objetos [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="6e459-114">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="6e459-115">Obter userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6e459-115">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="6e459-116">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6e459-116">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="6e459-117">Leia as propriedades e os relacionamentos do objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="6e459-117">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="6e459-118">Criar userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6e459-118">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="6e459-119">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6e459-119">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="6e459-120">Crie um novo objeto de [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="6e459-120">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="6e459-121">Excluir userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6e459-121">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="6e459-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e459-122">None</span></span>|<span data-ttu-id="6e459-123">Exclui um [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="6e459-123">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="6e459-124">Atualizar userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6e459-124">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="6e459-125">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6e459-125">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="6e459-126">Atualize as propriedades de um objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="6e459-126">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6e459-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e459-127">Properties</span></span>
|<span data-ttu-id="6e459-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e459-128">Property</span></span>|<span data-ttu-id="6e459-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e459-129">Type</span></span>|<span data-ttu-id="6e459-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e459-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e459-131">id</span><span class="sxs-lookup"><span data-stu-id="6e459-131">id</span></span>|<span data-ttu-id="6e459-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e459-132">String</span></span>|<span data-ttu-id="6e459-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6e459-133">Key of the entity.</span></span>|
|<span data-ttu-id="6e459-134">userName</span><span class="sxs-lookup"><span data-stu-id="6e459-134">userName</span></span>|<span data-ttu-id="6e459-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e459-135">String</span></span>|<span data-ttu-id="6e459-136">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="6e459-136">User name.</span></span>|
|<span data-ttu-id="6e459-137">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6e459-137">userPrincipalName</span></span>|<span data-ttu-id="6e459-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e459-138">String</span></span>|<span data-ttu-id="6e459-139">Nome Principal de usuário.</span><span class="sxs-lookup"><span data-stu-id="6e459-139">User Principal Name.</span></span>|
|<span data-ttu-id="6e459-140">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6e459-140">installedDeviceCount</span></span>|<span data-ttu-id="6e459-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6e459-141">Int32</span></span>|<span data-ttu-id="6e459-142">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="6e459-142">Installed Device Count.</span></span>|
|<span data-ttu-id="6e459-143">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6e459-143">failedDeviceCount</span></span>|<span data-ttu-id="6e459-144">Int32</span><span class="sxs-lookup"><span data-stu-id="6e459-144">Int32</span></span>|<span data-ttu-id="6e459-145">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6e459-145">Failed Device Count.</span></span>|
|<span data-ttu-id="6e459-146">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6e459-146">notInstalledDeviceCount</span></span>|<span data-ttu-id="6e459-147">Int32</span><span class="sxs-lookup"><span data-stu-id="6e459-147">Int32</span></span>|<span data-ttu-id="6e459-148">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="6e459-148">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e459-149">Relações</span><span class="sxs-lookup"><span data-stu-id="6e459-149">Relationships</span></span>
|<span data-ttu-id="6e459-150">Relação</span><span class="sxs-lookup"><span data-stu-id="6e459-150">Relationship</span></span>|<span data-ttu-id="6e459-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e459-151">Type</span></span>|<span data-ttu-id="6e459-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e459-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e459-153">app</span><span class="sxs-lookup"><span data-stu-id="6e459-153">app</span></span>|[<span data-ttu-id="6e459-154">mobileApp</span><span class="sxs-lookup"><span data-stu-id="6e459-154">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="6e459-155">O link de navegação para o aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="6e459-155">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="6e459-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="6e459-156">deviceStatuses</span></span>|<span data-ttu-id="6e459-157">coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="6e459-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="6e459-158">O estado de instalação do aplicativo em dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6e459-158">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e459-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e459-159">JSON Representation</span></span>
<span data-ttu-id="6e459-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e459-160">Here is a JSON representation of the resource.</span></span>
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





