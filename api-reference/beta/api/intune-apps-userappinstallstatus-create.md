---
title: Criar userAppInstallStatus
description: Criar um novo objeto userAppInstallStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 835329c8a73d8974ea13ff31456303d6b4cdffd7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761058"
---
# <a name="create-userappinstallstatus"></a><span data-ttu-id="7140d-103">Criar userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="7140d-103">Create userAppInstallStatus</span></span>

> <span data-ttu-id="7140d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7140d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7140d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7140d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7140d-106">Criar um novo objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="7140d-106">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7140d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7140d-107">Prerequisites</span></span>
<span data-ttu-id="7140d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7140d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7140d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7140d-110">Permission type</span></span>|<span data-ttu-id="7140d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7140d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7140d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7140d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7140d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7140d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7140d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7140d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7140d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7140d-115">Not supported.</span></span>|
|<span data-ttu-id="7140d-116">Application</span><span class="sxs-lookup"><span data-stu-id="7140d-116">Application</span></span>|<span data-ttu-id="7140d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7140d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7140d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7140d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="7140d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7140d-119">Request headers</span></span>
|<span data-ttu-id="7140d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7140d-120">Header</span></span>|<span data-ttu-id="7140d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7140d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7140d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7140d-122">Authorization</span></span>|<span data-ttu-id="7140d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7140d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7140d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7140d-124">Accept</span></span>|<span data-ttu-id="7140d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7140d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7140d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7140d-126">Request body</span></span>
<span data-ttu-id="7140d-127">No corpo da solicitação, forneça uma representação JSON do objeto userAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="7140d-127">In the request body, supply a JSON representation for the userAppInstallStatus object.</span></span>

<span data-ttu-id="7140d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar userAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="7140d-128">The following table shows the properties that are required when you create the userAppInstallStatus.</span></span>

|<span data-ttu-id="7140d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7140d-129">Property</span></span>|<span data-ttu-id="7140d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7140d-130">Type</span></span>|<span data-ttu-id="7140d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7140d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7140d-132">id</span><span class="sxs-lookup"><span data-stu-id="7140d-132">id</span></span>|<span data-ttu-id="7140d-133">String</span><span class="sxs-lookup"><span data-stu-id="7140d-133">String</span></span>|<span data-ttu-id="7140d-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7140d-134">Key of the entity.</span></span>|
|<span data-ttu-id="7140d-135">userName</span><span class="sxs-lookup"><span data-stu-id="7140d-135">userName</span></span>|<span data-ttu-id="7140d-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7140d-136">String</span></span>|<span data-ttu-id="7140d-137">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="7140d-137">User name.</span></span>|
|<span data-ttu-id="7140d-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7140d-138">userPrincipalName</span></span>|<span data-ttu-id="7140d-139">String</span><span class="sxs-lookup"><span data-stu-id="7140d-139">String</span></span>|<span data-ttu-id="7140d-140">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="7140d-140">User Principal Name.</span></span>|
|<span data-ttu-id="7140d-141">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7140d-141">installedDeviceCount</span></span>|<span data-ttu-id="7140d-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7140d-142">Int32</span></span>|<span data-ttu-id="7140d-143">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="7140d-143">Installed Device Count.</span></span>|
|<span data-ttu-id="7140d-144">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7140d-144">failedDeviceCount</span></span>|<span data-ttu-id="7140d-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7140d-145">Int32</span></span>|<span data-ttu-id="7140d-146">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="7140d-146">Failed Device Count.</span></span>|
|<span data-ttu-id="7140d-147">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7140d-147">notInstalledDeviceCount</span></span>|<span data-ttu-id="7140d-148">Int32</span><span class="sxs-lookup"><span data-stu-id="7140d-148">Int32</span></span>|<span data-ttu-id="7140d-149">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="7140d-149">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="7140d-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7140d-150">Response</span></span>
<span data-ttu-id="7140d-151">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7140d-151">If successful, this method returns a `201 Created` response code and a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7140d-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7140d-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="7140d-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7140d-153">Request</span></span>
<span data-ttu-id="7140d-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7140d-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
Content-type: application/json
Content-length: 239

{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="7140d-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="7140d-155">Response</span></span>
<span data-ttu-id="7140d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7140d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 288

{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "14959a2a-9a2a-1495-2a9a-95142a9a9514",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```




