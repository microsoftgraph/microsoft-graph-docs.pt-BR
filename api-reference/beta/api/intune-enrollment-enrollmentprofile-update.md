---
title: Atualizar enrollmentProfile
description: Atualiza as propriedades de um objeto enrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1029d87b5df14c79e7e93b849e4bd1caca1066e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141304"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="b9a39-103">Atualizar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="b9a39-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="b9a39-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9a39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9a39-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9a39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9a39-106">Atualiza as propriedades de um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b9a39-106">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9a39-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9a39-107">Prerequisites</span></span>
<span data-ttu-id="b9a39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b9a39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b9a39-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9a39-110">Permission type</span></span>|<span data-ttu-id="b9a39-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9a39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9a39-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9a39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9a39-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9a39-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b9a39-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9a39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9a39-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9a39-115">Not supported.</span></span>|
|<span data-ttu-id="b9a39-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9a39-116">Application</span></span>|<span data-ttu-id="b9a39-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9a39-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9a39-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9a39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="b9a39-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a39-119">Request headers</span></span>
|<span data-ttu-id="b9a39-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9a39-120">Header</span></span>|<span data-ttu-id="b9a39-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b9a39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9a39-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9a39-122">Authorization</span></span>|<span data-ttu-id="b9a39-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9a39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9a39-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9a39-124">Accept</span></span>|<span data-ttu-id="b9a39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9a39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9a39-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a39-126">Request body</span></span>
<span data-ttu-id="b9a39-127">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b9a39-127">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="b9a39-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="b9a39-128">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="b9a39-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9a39-129">Property</span></span>|<span data-ttu-id="b9a39-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9a39-130">Type</span></span>|<span data-ttu-id="b9a39-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9a39-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9a39-132">id</span><span class="sxs-lookup"><span data-stu-id="b9a39-132">id</span></span>|<span data-ttu-id="b9a39-133">String</span><span class="sxs-lookup"><span data-stu-id="b9a39-133">String</span></span>|<span data-ttu-id="b9a39-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="b9a39-134">The GUID for the object</span></span>|
|<span data-ttu-id="b9a39-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b9a39-135">displayName</span></span>|<span data-ttu-id="b9a39-136">String</span><span class="sxs-lookup"><span data-stu-id="b9a39-136">String</span></span>|<span data-ttu-id="b9a39-137">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="b9a39-137">Name of the profile</span></span>|
|<span data-ttu-id="b9a39-138">description</span><span class="sxs-lookup"><span data-stu-id="b9a39-138">description</span></span>|<span data-ttu-id="b9a39-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9a39-139">String</span></span>|<span data-ttu-id="b9a39-140">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="b9a39-140">Description of the profile</span></span>|
|<span data-ttu-id="b9a39-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="b9a39-141">requiresUserAuthentication</span></span>|<span data-ttu-id="b9a39-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="b9a39-142">Boolean</span></span>|<span data-ttu-id="b9a39-143">Indica se o perfil requer autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="b9a39-143">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="b9a39-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="b9a39-144">configurationEndpointUrl</span></span>|<span data-ttu-id="b9a39-145">String</span><span class="sxs-lookup"><span data-stu-id="b9a39-145">String</span></span>|<span data-ttu-id="b9a39-146">URL de ponto de extremidade de configuração a ser usada para registro</span><span class="sxs-lookup"><span data-stu-id="b9a39-146">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="b9a39-147">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="b9a39-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="b9a39-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="b9a39-148">Boolean</span></span>|<span data-ttu-id="b9a39-149">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="b9a39-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="b9a39-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="b9a39-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="b9a39-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="b9a39-151">Boolean</span></span>|<span data-ttu-id="b9a39-152">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados</span><span class="sxs-lookup"><span data-stu-id="b9a39-152">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="b9a39-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9a39-153">Response</span></span>
<span data-ttu-id="b9a39-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9a39-154">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9a39-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9a39-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9a39-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a39-156">Request</span></span>
<span data-ttu-id="b9a39-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9a39-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 370

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```

### <a name="response"></a><span data-ttu-id="b9a39-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9a39-158">Response</span></span>
<span data-ttu-id="b9a39-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9a39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 419

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```




