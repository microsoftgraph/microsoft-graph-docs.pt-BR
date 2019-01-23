---
title: Criar userAppInstallStatus
description: Crie um novo objeto de userAppInstallStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3ebb03db9e8d9f0c2eab30ecebbee4dbf8832654
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397866"
---
# <a name="create-userappinstallstatus"></a><span data-ttu-id="70b2c-103">Criar userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="70b2c-103">Create userAppInstallStatus</span></span>

> <span data-ttu-id="70b2c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="70b2c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="70b2c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="70b2c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70b2c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="70b2c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70b2c-107">Crie um novo objeto de [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="70b2c-107">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70b2c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="70b2c-108">Prerequisites</span></span>
<span data-ttu-id="70b2c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="70b2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="70b2c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70b2c-111">Permission type</span></span>|<span data-ttu-id="70b2c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="70b2c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70b2c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70b2c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70b2c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70b2c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="70b2c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70b2c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70b2c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70b2c-116">Not supported.</span></span>|
|<span data-ttu-id="70b2c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70b2c-117">Application</span></span>|<span data-ttu-id="70b2c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70b2c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70b2c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70b2c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="70b2c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70b2c-120">Request headers</span></span>
|<span data-ttu-id="70b2c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="70b2c-121">Header</span></span>|<span data-ttu-id="70b2c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="70b2c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70b2c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="70b2c-123">Authorization</span></span>|<span data-ttu-id="70b2c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70b2c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70b2c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="70b2c-125">Accept</span></span>|<span data-ttu-id="70b2c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70b2c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70b2c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70b2c-127">Request body</span></span>
<span data-ttu-id="70b2c-128">No corpo da solicitação, fornece uma representação JSON para o objeto userAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="70b2c-128">In the request body, supply a JSON representation for the userAppInstallStatus object.</span></span>

<span data-ttu-id="70b2c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o userAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="70b2c-129">The following table shows the properties that are required when you create the userAppInstallStatus.</span></span>

|<span data-ttu-id="70b2c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70b2c-130">Property</span></span>|<span data-ttu-id="70b2c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="70b2c-131">Type</span></span>|<span data-ttu-id="70b2c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="70b2c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70b2c-133">id</span><span class="sxs-lookup"><span data-stu-id="70b2c-133">id</span></span>|<span data-ttu-id="70b2c-134">String</span><span class="sxs-lookup"><span data-stu-id="70b2c-134">String</span></span>|<span data-ttu-id="70b2c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="70b2c-135">Key of the entity.</span></span>|
|<span data-ttu-id="70b2c-136">userName</span><span class="sxs-lookup"><span data-stu-id="70b2c-136">userName</span></span>|<span data-ttu-id="70b2c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70b2c-137">String</span></span>|<span data-ttu-id="70b2c-138">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="70b2c-138">User name.</span></span>|
|<span data-ttu-id="70b2c-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="70b2c-139">userPrincipalName</span></span>|<span data-ttu-id="70b2c-140">String</span><span class="sxs-lookup"><span data-stu-id="70b2c-140">String</span></span>|<span data-ttu-id="70b2c-141">Nome Principal de usuário.</span><span class="sxs-lookup"><span data-stu-id="70b2c-141">User Principal Name.</span></span>|
|<span data-ttu-id="70b2c-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70b2c-142">installedDeviceCount</span></span>|<span data-ttu-id="70b2c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="70b2c-143">Int32</span></span>|<span data-ttu-id="70b2c-144">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="70b2c-144">Installed Device Count.</span></span>|
|<span data-ttu-id="70b2c-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70b2c-145">failedDeviceCount</span></span>|<span data-ttu-id="70b2c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="70b2c-146">Int32</span></span>|<span data-ttu-id="70b2c-147">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="70b2c-147">Failed Device Count.</span></span>|
|<span data-ttu-id="70b2c-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70b2c-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="70b2c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="70b2c-149">Int32</span></span>|<span data-ttu-id="70b2c-150">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="70b2c-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="70b2c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="70b2c-151">Response</span></span>
<span data-ttu-id="70b2c-152">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70b2c-152">If successful, this method returns a `201 Created` response code and a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70b2c-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70b2c-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="70b2c-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70b2c-154">Request</span></span>
<span data-ttu-id="70b2c-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70b2c-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="70b2c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="70b2c-156">Response</span></span>
<span data-ttu-id="70b2c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70b2c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




