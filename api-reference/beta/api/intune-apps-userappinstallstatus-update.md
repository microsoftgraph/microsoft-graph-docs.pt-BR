---
title: Atualizar userAppInstallStatus
description: Atualiza as propriedades de um objeto userAppInstallStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ab2e6e095c97d17672c694d3a827791405f1a076
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960352"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="2e246-103">Atualizar userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="2e246-103">Update userAppInstallStatus</span></span>

> <span data-ttu-id="2e246-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2e246-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e246-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2e246-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e246-106">Atualiza as propriedades de um objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="2e246-106">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e246-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2e246-107">Prerequisites</span></span>
<span data-ttu-id="2e246-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e246-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e246-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e246-110">Permission type</span></span>|<span data-ttu-id="2e246-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2e246-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e246-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e246-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2e246-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e246-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2e246-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e246-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e246-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e246-115">Not supported.</span></span>|
|<span data-ttu-id="2e246-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e246-116">Application</span></span>|<span data-ttu-id="2e246-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e246-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e246-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e246-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="2e246-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e246-119">Request headers</span></span>
|<span data-ttu-id="2e246-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2e246-120">Header</span></span>|<span data-ttu-id="2e246-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2e246-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e246-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e246-122">Authorization</span></span>|<span data-ttu-id="2e246-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e246-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e246-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2e246-124">Accept</span></span>|<span data-ttu-id="2e246-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2e246-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e246-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e246-126">Request body</span></span>
<span data-ttu-id="2e246-127">No corpo da solicitação, forneça uma representação JSON do objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="2e246-127">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="2e246-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="2e246-128">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="2e246-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e246-129">Property</span></span>|<span data-ttu-id="2e246-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e246-130">Type</span></span>|<span data-ttu-id="2e246-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e246-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e246-132">id</span><span class="sxs-lookup"><span data-stu-id="2e246-132">id</span></span>|<span data-ttu-id="2e246-133">String</span><span class="sxs-lookup"><span data-stu-id="2e246-133">String</span></span>|<span data-ttu-id="2e246-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2e246-134">Key of the entity.</span></span>|
|<span data-ttu-id="2e246-135">userName</span><span class="sxs-lookup"><span data-stu-id="2e246-135">userName</span></span>|<span data-ttu-id="2e246-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e246-136">String</span></span>|<span data-ttu-id="2e246-137">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="2e246-137">User name.</span></span>|
|<span data-ttu-id="2e246-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2e246-138">userPrincipalName</span></span>|<span data-ttu-id="2e246-139">String</span><span class="sxs-lookup"><span data-stu-id="2e246-139">String</span></span>|<span data-ttu-id="2e246-140">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="2e246-140">User Principal Name.</span></span>|
|<span data-ttu-id="2e246-141">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2e246-141">installedDeviceCount</span></span>|<span data-ttu-id="2e246-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2e246-142">Int32</span></span>|<span data-ttu-id="2e246-143">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="2e246-143">Installed Device Count.</span></span>|
|<span data-ttu-id="2e246-144">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2e246-144">failedDeviceCount</span></span>|<span data-ttu-id="2e246-145">Int32</span><span class="sxs-lookup"><span data-stu-id="2e246-145">Int32</span></span>|<span data-ttu-id="2e246-146">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2e246-146">Failed Device Count.</span></span>|
|<span data-ttu-id="2e246-147">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2e246-147">notInstalledDeviceCount</span></span>|<span data-ttu-id="2e246-148">Int32</span><span class="sxs-lookup"><span data-stu-id="2e246-148">Int32</span></span>|<span data-ttu-id="2e246-149">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="2e246-149">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="2e246-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e246-150">Response</span></span>
<span data-ttu-id="2e246-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e246-151">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e246-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e246-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e246-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e246-153">Request</span></span>
<span data-ttu-id="2e246-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e246-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
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

### <a name="response"></a><span data-ttu-id="2e246-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e246-155">Response</span></span>
<span data-ttu-id="2e246-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e246-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





