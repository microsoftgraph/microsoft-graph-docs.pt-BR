---
title: Criar userAppInstallStatus
description: Crie um novo objeto userAppInstallStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c8d83cbaa989a811226b8227e5f62d045365ce81
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142965"
---
# <a name="create-userappinstallstatus"></a><span data-ttu-id="7c709-103">Criar userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="7c709-103">Create userAppInstallStatus</span></span>

<span data-ttu-id="7c709-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c709-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c709-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c709-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c709-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c709-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c709-107">Crie um novo [objeto userAppInstallStatus.](../resources/intune-apps-userappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="7c709-107">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c709-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c709-108">Prerequisites</span></span>
<span data-ttu-id="7c709-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c709-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c709-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c709-111">Permission type</span></span>|<span data-ttu-id="7c709-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c709-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c709-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c709-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c709-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c709-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7c709-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c709-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c709-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c709-116">Not supported.</span></span>|
|<span data-ttu-id="7c709-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c709-117">Application</span></span>|<span data-ttu-id="7c709-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c709-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c709-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c709-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="7c709-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c709-120">Request headers</span></span>
|<span data-ttu-id="7c709-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c709-121">Header</span></span>|<span data-ttu-id="7c709-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7c709-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c709-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c709-123">Authorization</span></span>|<span data-ttu-id="7c709-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c709-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c709-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c709-125">Accept</span></span>|<span data-ttu-id="7c709-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c709-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c709-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c709-127">Request body</span></span>
<span data-ttu-id="7c709-128">No corpo da solicitação, fornece uma representação JSON para o objeto userAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="7c709-128">In the request body, supply a JSON representation for the userAppInstallStatus object.</span></span>

<span data-ttu-id="7c709-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o userAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="7c709-129">The following table shows the properties that are required when you create the userAppInstallStatus.</span></span>

|<span data-ttu-id="7c709-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c709-130">Property</span></span>|<span data-ttu-id="7c709-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c709-131">Type</span></span>|<span data-ttu-id="7c709-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c709-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c709-133">id</span><span class="sxs-lookup"><span data-stu-id="7c709-133">id</span></span>|<span data-ttu-id="7c709-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c709-134">String</span></span>|<span data-ttu-id="7c709-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7c709-135">Key of the entity.</span></span>|
|<span data-ttu-id="7c709-136">userName</span><span class="sxs-lookup"><span data-stu-id="7c709-136">userName</span></span>|<span data-ttu-id="7c709-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c709-137">String</span></span>|<span data-ttu-id="7c709-138">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="7c709-138">User name.</span></span>|
|<span data-ttu-id="7c709-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7c709-139">userPrincipalName</span></span>|<span data-ttu-id="7c709-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c709-140">String</span></span>|<span data-ttu-id="7c709-141">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="7c709-141">User Principal Name.</span></span>|
|<span data-ttu-id="7c709-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7c709-142">installedDeviceCount</span></span>|<span data-ttu-id="7c709-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7c709-143">Int32</span></span>|<span data-ttu-id="7c709-144">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="7c709-144">Installed Device Count.</span></span>|
|<span data-ttu-id="7c709-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7c709-145">failedDeviceCount</span></span>|<span data-ttu-id="7c709-146">Int32</span><span class="sxs-lookup"><span data-stu-id="7c709-146">Int32</span></span>|<span data-ttu-id="7c709-147">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="7c709-147">Failed Device Count.</span></span>|
|<span data-ttu-id="7c709-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7c709-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="7c709-149">Int32</span><span class="sxs-lookup"><span data-stu-id="7c709-149">Int32</span></span>|<span data-ttu-id="7c709-150">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="7c709-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="7c709-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c709-151">Response</span></span>
<span data-ttu-id="7c709-152">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c709-152">If successful, this method returns a `201 Created` response code and a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c709-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c709-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c709-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c709-154">Request</span></span>
<span data-ttu-id="7c709-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c709-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c709-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c709-156">Response</span></span>
<span data-ttu-id="7c709-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c709-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




