---
title: tipo de recurso de userAppInstallStatus
description: Contém propriedades para o status de instalação de um usuário.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1e1369e35af2343bebd609c760075a830649a1f2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399889"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="ac1eb-103">tipo de recurso de userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ac1eb-103">userAppInstallStatus resource type</span></span>

> <span data-ttu-id="ac1eb-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ac1eb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ac1eb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ac1eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ac1eb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ac1eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac1eb-107">Contém propriedades para o status de instalação de um usuário.</span><span class="sxs-lookup"><span data-stu-id="ac1eb-107">Contains properties for the installation status for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="ac1eb-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="ac1eb-108">Methods</span></span>
|<span data-ttu-id="ac1eb-109">Método</span><span class="sxs-lookup"><span data-stu-id="ac1eb-109">Method</span></span>|<span data-ttu-id="ac1eb-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ac1eb-110">Return Type</span></span>|<span data-ttu-id="ac1eb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac1eb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ac1eb-112">Lista userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="ac1eb-112">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="ac1eb-113">coleção [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="ac1eb-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="ac1eb-114">Lista as propriedades e os relacionamentos dos objetos [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="ac1eb-114">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="ac1eb-115">Obter userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ac1eb-115">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="ac1eb-116">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ac1eb-116">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="ac1eb-117">Leia as propriedades e os relacionamentos do objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="ac1eb-117">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="ac1eb-118">Criar userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ac1eb-118">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="ac1eb-119">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ac1eb-119">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="ac1eb-120">Crie um novo objeto de [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="ac1eb-120">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="ac1eb-121">Excluir userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ac1eb-121">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="ac1eb-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac1eb-122">None</span></span>|<span data-ttu-id="ac1eb-123">Exclui um [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="ac1eb-123">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="ac1eb-124">Atualizar userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ac1eb-124">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="ac1eb-125">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ac1eb-125">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="ac1eb-126">Atualize as propriedades de um objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="ac1eb-126">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ac1eb-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac1eb-127">Properties</span></span>
|<span data-ttu-id="ac1eb-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac1eb-128">Property</span></span>|<span data-ttu-id="ac1eb-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac1eb-129">Type</span></span>|<span data-ttu-id="ac1eb-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac1eb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac1eb-131">id</span><span class="sxs-lookup"><span data-stu-id="ac1eb-131">id</span></span>|<span data-ttu-id="ac1eb-132">String</span><span class="sxs-lookup"><span data-stu-id="ac1eb-132">String</span></span>|<span data-ttu-id="ac1eb-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ac1eb-133">Key of the entity.</span></span>|
|<span data-ttu-id="ac1eb-134">userName</span><span class="sxs-lookup"><span data-stu-id="ac1eb-134">userName</span></span>|<span data-ttu-id="ac1eb-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac1eb-135">String</span></span>|<span data-ttu-id="ac1eb-136">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="ac1eb-136">User name.</span></span>|
|<span data-ttu-id="ac1eb-137">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ac1eb-137">userPrincipalName</span></span>|<span data-ttu-id="ac1eb-138">String</span><span class="sxs-lookup"><span data-stu-id="ac1eb-138">String</span></span>|<span data-ttu-id="ac1eb-139">Nome Principal de usuário.</span><span class="sxs-lookup"><span data-stu-id="ac1eb-139">User Principal Name.</span></span>|
|<span data-ttu-id="ac1eb-140">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ac1eb-140">installedDeviceCount</span></span>|<span data-ttu-id="ac1eb-141">Int32</span><span class="sxs-lookup"><span data-stu-id="ac1eb-141">Int32</span></span>|<span data-ttu-id="ac1eb-142">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="ac1eb-142">Installed Device Count.</span></span>|
|<span data-ttu-id="ac1eb-143">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ac1eb-143">failedDeviceCount</span></span>|<span data-ttu-id="ac1eb-144">Int32</span><span class="sxs-lookup"><span data-stu-id="ac1eb-144">Int32</span></span>|<span data-ttu-id="ac1eb-145">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ac1eb-145">Failed Device Count.</span></span>|
|<span data-ttu-id="ac1eb-146">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ac1eb-146">notInstalledDeviceCount</span></span>|<span data-ttu-id="ac1eb-147">Int32</span><span class="sxs-lookup"><span data-stu-id="ac1eb-147">Int32</span></span>|<span data-ttu-id="ac1eb-148">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="ac1eb-148">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac1eb-149">Relações</span><span class="sxs-lookup"><span data-stu-id="ac1eb-149">Relationships</span></span>
|<span data-ttu-id="ac1eb-150">Relação</span><span class="sxs-lookup"><span data-stu-id="ac1eb-150">Relationship</span></span>|<span data-ttu-id="ac1eb-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac1eb-151">Type</span></span>|<span data-ttu-id="ac1eb-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac1eb-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac1eb-153">app</span><span class="sxs-lookup"><span data-stu-id="ac1eb-153">app</span></span>|[<span data-ttu-id="ac1eb-154">mobileApp</span><span class="sxs-lookup"><span data-stu-id="ac1eb-154">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="ac1eb-155">O link de navegação para o aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="ac1eb-155">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="ac1eb-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="ac1eb-156">deviceStatuses</span></span>|<span data-ttu-id="ac1eb-157">coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="ac1eb-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="ac1eb-158">O estado de instalação do aplicativo em dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ac1eb-158">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac1eb-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac1eb-159">JSON Representation</span></span>
<span data-ttu-id="ac1eb-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac1eb-160">Here is a JSON representation of the resource.</span></span>
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




