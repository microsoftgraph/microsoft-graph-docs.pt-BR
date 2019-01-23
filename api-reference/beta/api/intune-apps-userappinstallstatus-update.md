---
title: Atualizar userAppInstallStatus
description: Atualize as propriedades de um objeto userAppInstallStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 237e9f28f36fb25ea5ddad46f5a6a75242767c6b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413833"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="cff99-103">Atualizar userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="cff99-103">Update userAppInstallStatus</span></span>

> <span data-ttu-id="cff99-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cff99-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cff99-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cff99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cff99-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cff99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cff99-107">Atualize as propriedades de um objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="cff99-107">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cff99-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cff99-108">Prerequisites</span></span>
<span data-ttu-id="cff99-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cff99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cff99-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cff99-111">Permission type</span></span>|<span data-ttu-id="cff99-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cff99-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cff99-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cff99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cff99-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cff99-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cff99-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cff99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cff99-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cff99-116">Not supported.</span></span>|
|<span data-ttu-id="cff99-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cff99-117">Application</span></span>|<span data-ttu-id="cff99-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cff99-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cff99-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cff99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="cff99-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cff99-120">Request headers</span></span>
|<span data-ttu-id="cff99-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cff99-121">Header</span></span>|<span data-ttu-id="cff99-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cff99-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cff99-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cff99-123">Authorization</span></span>|<span data-ttu-id="cff99-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cff99-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cff99-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cff99-125">Accept</span></span>|<span data-ttu-id="cff99-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cff99-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cff99-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cff99-127">Request body</span></span>
<span data-ttu-id="cff99-128">No corpo da solicitação, fornece uma representação JSON para o objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="cff99-128">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="cff99-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="cff99-129">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="cff99-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cff99-130">Property</span></span>|<span data-ttu-id="cff99-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cff99-131">Type</span></span>|<span data-ttu-id="cff99-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cff99-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cff99-133">id</span><span class="sxs-lookup"><span data-stu-id="cff99-133">id</span></span>|<span data-ttu-id="cff99-134">String</span><span class="sxs-lookup"><span data-stu-id="cff99-134">String</span></span>|<span data-ttu-id="cff99-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cff99-135">Key of the entity.</span></span>|
|<span data-ttu-id="cff99-136">userName</span><span class="sxs-lookup"><span data-stu-id="cff99-136">userName</span></span>|<span data-ttu-id="cff99-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cff99-137">String</span></span>|<span data-ttu-id="cff99-138">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="cff99-138">User name.</span></span>|
|<span data-ttu-id="cff99-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cff99-139">userPrincipalName</span></span>|<span data-ttu-id="cff99-140">String</span><span class="sxs-lookup"><span data-stu-id="cff99-140">String</span></span>|<span data-ttu-id="cff99-141">Nome Principal de usuário.</span><span class="sxs-lookup"><span data-stu-id="cff99-141">User Principal Name.</span></span>|
|<span data-ttu-id="cff99-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cff99-142">installedDeviceCount</span></span>|<span data-ttu-id="cff99-143">Int32</span><span class="sxs-lookup"><span data-stu-id="cff99-143">Int32</span></span>|<span data-ttu-id="cff99-144">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="cff99-144">Installed Device Count.</span></span>|
|<span data-ttu-id="cff99-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cff99-145">failedDeviceCount</span></span>|<span data-ttu-id="cff99-146">Int32</span><span class="sxs-lookup"><span data-stu-id="cff99-146">Int32</span></span>|<span data-ttu-id="cff99-147">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="cff99-147">Failed Device Count.</span></span>|
|<span data-ttu-id="cff99-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cff99-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="cff99-149">Int32</span><span class="sxs-lookup"><span data-stu-id="cff99-149">Int32</span></span>|<span data-ttu-id="cff99-150">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="cff99-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="cff99-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="cff99-151">Response</span></span>
<span data-ttu-id="cff99-152">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cff99-152">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cff99-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cff99-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="cff99-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cff99-154">Request</span></span>
<span data-ttu-id="cff99-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cff99-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cff99-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="cff99-156">Response</span></span>
<span data-ttu-id="cff99-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cff99-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




