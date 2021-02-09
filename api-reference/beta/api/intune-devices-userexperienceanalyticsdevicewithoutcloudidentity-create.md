---
title: Criar userExperienceAnalyticsDeviceWithoutCloudIdentity
description: Crie um novo objeto userExperienceAnalyticsDeviceWithoutCloudIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a3022153d740837f0c05864decfb2caba8fc9a43
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162195"
---
# <a name="create-userexperienceanalyticsdevicewithoutcloudidentity"></a><span data-ttu-id="6663a-103">Criar userExperienceAnalyticsDeviceWithoutCloudIdentity</span><span class="sxs-lookup"><span data-stu-id="6663a-103">Create userExperienceAnalyticsDeviceWithoutCloudIdentity</span></span>

<span data-ttu-id="6663a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6663a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6663a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6663a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6663a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6663a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6663a-107">Crie um novo [objeto userExperienceAnalyticsDeviceWithoutCloudIdentity.](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)</span><span class="sxs-lookup"><span data-stu-id="6663a-107">Create a new [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6663a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6663a-108">Prerequisites</span></span>
<span data-ttu-id="6663a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6663a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6663a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6663a-111">Permission type</span></span>|<span data-ttu-id="6663a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6663a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6663a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6663a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6663a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6663a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6663a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6663a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6663a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6663a-116">Not supported.</span></span>|
|<span data-ttu-id="6663a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6663a-117">Application</span></span>|<span data-ttu-id="6663a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6663a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6663a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6663a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDevicesWithoutCloudIdentity
```

## <a name="request-headers"></a><span data-ttu-id="6663a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6663a-120">Request headers</span></span>
|<span data-ttu-id="6663a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6663a-121">Header</span></span>|<span data-ttu-id="6663a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6663a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6663a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6663a-123">Authorization</span></span>|<span data-ttu-id="6663a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6663a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6663a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6663a-125">Accept</span></span>|<span data-ttu-id="6663a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6663a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6663a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6663a-127">Request body</span></span>
<span data-ttu-id="6663a-128">No corpo da solicitação, fornece uma representação JSON do objeto userExperienceAnalyticsDeviceWithoutCloudIdentity.</span><span class="sxs-lookup"><span data-stu-id="6663a-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceWithoutCloudIdentity object.</span></span>

<span data-ttu-id="6663a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsDeviceWithoutCloudIdentity.</span><span class="sxs-lookup"><span data-stu-id="6663a-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceWithoutCloudIdentity.</span></span>

|<span data-ttu-id="6663a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6663a-130">Property</span></span>|<span data-ttu-id="6663a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6663a-131">Type</span></span>|<span data-ttu-id="6663a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6663a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6663a-133">id</span><span class="sxs-lookup"><span data-stu-id="6663a-133">id</span></span>|<span data-ttu-id="6663a-134">String</span><span class="sxs-lookup"><span data-stu-id="6663a-134">String</span></span>|<span data-ttu-id="6663a-135">O identificador exclusivo do dispositivo de anexação de locatário da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6663a-135">The unique identifier of the user experience analytics tenant attach device.</span></span>|
|<span data-ttu-id="6663a-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="6663a-136">deviceName</span></span>|<span data-ttu-id="6663a-137">String</span><span class="sxs-lookup"><span data-stu-id="6663a-137">String</span></span>|<span data-ttu-id="6663a-138">O nome do dispositivo de anexação de locatário.</span><span class="sxs-lookup"><span data-stu-id="6663a-138">The tenant attach device's name.</span></span>|
|<span data-ttu-id="6663a-139">azureAdDeviceId</span><span class="sxs-lookup"><span data-stu-id="6663a-139">azureAdDeviceId</span></span>|<span data-ttu-id="6663a-140">String</span><span class="sxs-lookup"><span data-stu-id="6663a-140">String</span></span>|<span data-ttu-id="6663a-141">ID de dispositivo do Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="6663a-141">Azure Active Directory Device Id</span></span>|



## <a name="response"></a><span data-ttu-id="6663a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6663a-142">Response</span></span>
<span data-ttu-id="6663a-143">Se tiver êxito, este método retornará um código de resposta e um objeto `201 Created` [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6663a-143">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6663a-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6663a-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="6663a-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6663a-145">Request</span></span>
<span data-ttu-id="6663a-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6663a-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicesWithoutCloudIdentity
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceWithoutCloudIdentity",
  "deviceName": "Device Name value",
  "azureAdDeviceId": "Azure Ad Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="6663a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="6663a-147">Response</span></span>
<span data-ttu-id="6663a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6663a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceWithoutCloudIdentity",
  "id": "80537287-7287-8053-8772-538087725380",
  "deviceName": "Device Name value",
  "azureAdDeviceId": "Azure Ad Device Id value"
}
```




