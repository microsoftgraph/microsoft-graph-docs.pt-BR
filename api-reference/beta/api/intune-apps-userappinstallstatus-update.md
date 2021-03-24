---
title: Atualizar userAppInstallStatus
description: Atualize as propriedades de um objeto userAppInstallStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10bd4b5a9064036e6e3d40fb4ac6334f8aada1d9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142951"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="3cd65-103">Atualizar userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="3cd65-103">Update userAppInstallStatus</span></span>

<span data-ttu-id="3cd65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cd65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3cd65-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3cd65-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cd65-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3cd65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cd65-107">Atualize as propriedades de um [objeto userAppInstallStatus.](../resources/intune-apps-userappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="3cd65-107">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3cd65-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3cd65-108">Prerequisites</span></span>
<span data-ttu-id="3cd65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cd65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cd65-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cd65-111">Permission type</span></span>|<span data-ttu-id="3cd65-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cd65-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cd65-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cd65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3cd65-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cd65-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3cd65-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cd65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cd65-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cd65-116">Not supported.</span></span>|
|<span data-ttu-id="3cd65-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cd65-117">Application</span></span>|<span data-ttu-id="3cd65-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cd65-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cd65-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cd65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="3cd65-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd65-120">Request headers</span></span>
|<span data-ttu-id="3cd65-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3cd65-121">Header</span></span>|<span data-ttu-id="3cd65-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3cd65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cd65-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cd65-123">Authorization</span></span>|<span data-ttu-id="3cd65-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cd65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cd65-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3cd65-125">Accept</span></span>|<span data-ttu-id="3cd65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3cd65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cd65-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd65-127">Request body</span></span>
<span data-ttu-id="3cd65-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userAppInstallStatus.](../resources/intune-apps-userappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="3cd65-128">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="3cd65-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="3cd65-129">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="3cd65-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3cd65-130">Property</span></span>|<span data-ttu-id="3cd65-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cd65-131">Type</span></span>|<span data-ttu-id="3cd65-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cd65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cd65-133">id</span><span class="sxs-lookup"><span data-stu-id="3cd65-133">id</span></span>|<span data-ttu-id="3cd65-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3cd65-134">String</span></span>|<span data-ttu-id="3cd65-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3cd65-135">Key of the entity.</span></span>|
|<span data-ttu-id="3cd65-136">userName</span><span class="sxs-lookup"><span data-stu-id="3cd65-136">userName</span></span>|<span data-ttu-id="3cd65-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3cd65-137">String</span></span>|<span data-ttu-id="3cd65-138">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="3cd65-138">User name.</span></span>|
|<span data-ttu-id="3cd65-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3cd65-139">userPrincipalName</span></span>|<span data-ttu-id="3cd65-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3cd65-140">String</span></span>|<span data-ttu-id="3cd65-141">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="3cd65-141">User Principal Name.</span></span>|
|<span data-ttu-id="3cd65-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3cd65-142">installedDeviceCount</span></span>|<span data-ttu-id="3cd65-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3cd65-143">Int32</span></span>|<span data-ttu-id="3cd65-144">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="3cd65-144">Installed Device Count.</span></span>|
|<span data-ttu-id="3cd65-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3cd65-145">failedDeviceCount</span></span>|<span data-ttu-id="3cd65-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3cd65-146">Int32</span></span>|<span data-ttu-id="3cd65-147">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="3cd65-147">Failed Device Count.</span></span>|
|<span data-ttu-id="3cd65-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3cd65-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="3cd65-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3cd65-149">Int32</span></span>|<span data-ttu-id="3cd65-150">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="3cd65-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="3cd65-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cd65-151">Response</span></span>
<span data-ttu-id="3cd65-152">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cd65-152">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cd65-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cd65-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cd65-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd65-154">Request</span></span>
<span data-ttu-id="3cd65-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cd65-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3cd65-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cd65-156">Response</span></span>
<span data-ttu-id="3cd65-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3cd65-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




