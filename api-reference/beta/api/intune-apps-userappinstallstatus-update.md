---
title: Atualizar userAppInstallStatus
description: Atualize as propriedades de um objeto userAppInstallStatus.
ms.openlocfilehash: 352ba84a5829132c78d9a3c4636531978da95d41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034050"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="f57f7-103">Atualizar userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="f57f7-103">Update userAppInstallStatus</span></span>

> <span data-ttu-id="f57f7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f57f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f57f7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f57f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f57f7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f57f7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f57f7-107">Atualize as propriedades de um objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="f57f7-107">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f57f7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f57f7-108">Prerequisites</span></span>
<span data-ttu-id="f57f7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f57f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f57f7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f57f7-111">Permission type</span></span>|<span data-ttu-id="f57f7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f57f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f57f7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f57f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f57f7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f57f7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f57f7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f57f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f57f7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f57f7-116">Not supported.</span></span>|
|<span data-ttu-id="f57f7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f57f7-117">Application</span></span>|<span data-ttu-id="f57f7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f57f7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f57f7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f57f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="f57f7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f57f7-120">Request headers</span></span>
|<span data-ttu-id="f57f7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f57f7-121">Header</span></span>|<span data-ttu-id="f57f7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f57f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f57f7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f57f7-123">Authorization</span></span>|<span data-ttu-id="f57f7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f57f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f57f7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f57f7-125">Accept</span></span>|<span data-ttu-id="f57f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f57f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f57f7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f57f7-127">Request body</span></span>
<span data-ttu-id="f57f7-128">No corpo da solicitação, fornece uma representação JSON para o objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="f57f7-128">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="f57f7-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f57f7-129">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="f57f7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f57f7-130">Property</span></span>|<span data-ttu-id="f57f7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f57f7-131">Type</span></span>|<span data-ttu-id="f57f7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f57f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f57f7-133">id</span><span class="sxs-lookup"><span data-stu-id="f57f7-133">id</span></span>|<span data-ttu-id="f57f7-134">String</span><span class="sxs-lookup"><span data-stu-id="f57f7-134">String</span></span>|<span data-ttu-id="f57f7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f57f7-135">Key of the entity.</span></span>|
|<span data-ttu-id="f57f7-136">userName</span><span class="sxs-lookup"><span data-stu-id="f57f7-136">userName</span></span>|<span data-ttu-id="f57f7-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f57f7-137">String</span></span>|<span data-ttu-id="f57f7-138">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="f57f7-138">User name.</span></span>|
|<span data-ttu-id="f57f7-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f57f7-139">userPrincipalName</span></span>|<span data-ttu-id="f57f7-140">String</span><span class="sxs-lookup"><span data-stu-id="f57f7-140">String</span></span>|<span data-ttu-id="f57f7-141">Nome Principal de usuário.</span><span class="sxs-lookup"><span data-stu-id="f57f7-141">User Principal Name.</span></span>|
|<span data-ttu-id="f57f7-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f57f7-142">installedDeviceCount</span></span>|<span data-ttu-id="f57f7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f57f7-143">Int32</span></span>|<span data-ttu-id="f57f7-144">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="f57f7-144">Installed Device Count.</span></span>|
|<span data-ttu-id="f57f7-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f57f7-145">failedDeviceCount</span></span>|<span data-ttu-id="f57f7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f57f7-146">Int32</span></span>|<span data-ttu-id="f57f7-147">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f57f7-147">Failed Device Count.</span></span>|
|<span data-ttu-id="f57f7-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f57f7-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="f57f7-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f57f7-149">Int32</span></span>|<span data-ttu-id="f57f7-150">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="f57f7-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="f57f7-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="f57f7-151">Response</span></span>
<span data-ttu-id="f57f7-152">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f57f7-152">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f57f7-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f57f7-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="f57f7-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f57f7-154">Request</span></span>
<span data-ttu-id="f57f7-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f57f7-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
Content-type: application/json
Content-length: 180

{
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="f57f7-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="f57f7-156">Response</span></span>
<span data-ttu-id="f57f7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f57f7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





