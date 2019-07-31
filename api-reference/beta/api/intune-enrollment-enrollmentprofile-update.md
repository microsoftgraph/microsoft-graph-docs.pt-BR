---
title: Atualizar enrollmentProfile
description: Atualiza as propriedades de um objeto enrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a7a34c7e571eadda316631937a718d5907096dab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985109"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="81218-103">Atualizar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="81218-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="81218-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81218-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81218-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81218-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81218-106">Atualiza as propriedades de um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="81218-106">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81218-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81218-107">Prerequisites</span></span>
<span data-ttu-id="81218-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81218-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81218-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81218-110">Permission type</span></span>|<span data-ttu-id="81218-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81218-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81218-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81218-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81218-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81218-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="81218-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81218-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81218-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81218-115">Not supported.</span></span>|
|<span data-ttu-id="81218-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81218-116">Application</span></span>|<span data-ttu-id="81218-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81218-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81218-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81218-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="81218-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81218-119">Request headers</span></span>
|<span data-ttu-id="81218-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81218-120">Header</span></span>|<span data-ttu-id="81218-121">Valor</span><span class="sxs-lookup"><span data-stu-id="81218-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81218-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="81218-122">Authorization</span></span>|<span data-ttu-id="81218-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81218-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81218-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81218-124">Accept</span></span>|<span data-ttu-id="81218-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81218-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81218-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81218-126">Request body</span></span>
<span data-ttu-id="81218-127">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="81218-127">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="81218-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="81218-128">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="81218-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81218-129">Property</span></span>|<span data-ttu-id="81218-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="81218-130">Type</span></span>|<span data-ttu-id="81218-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="81218-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81218-132">id</span><span class="sxs-lookup"><span data-stu-id="81218-132">id</span></span>|<span data-ttu-id="81218-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81218-133">String</span></span>|<span data-ttu-id="81218-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="81218-134">The GUID for the object</span></span>|
|<span data-ttu-id="81218-135">displayName</span><span class="sxs-lookup"><span data-stu-id="81218-135">displayName</span></span>|<span data-ttu-id="81218-136">String</span><span class="sxs-lookup"><span data-stu-id="81218-136">String</span></span>|<span data-ttu-id="81218-137">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="81218-137">Name of the profile</span></span>|
|<span data-ttu-id="81218-138">descrição</span><span class="sxs-lookup"><span data-stu-id="81218-138">description</span></span>|<span data-ttu-id="81218-139">String</span><span class="sxs-lookup"><span data-stu-id="81218-139">String</span></span>|<span data-ttu-id="81218-140">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="81218-140">Description of the profile</span></span>|
|<span data-ttu-id="81218-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="81218-141">requiresUserAuthentication</span></span>|<span data-ttu-id="81218-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="81218-142">Boolean</span></span>|<span data-ttu-id="81218-143">Indica se o perfil requer autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="81218-143">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="81218-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="81218-144">configurationEndpointUrl</span></span>|<span data-ttu-id="81218-145">String</span><span class="sxs-lookup"><span data-stu-id="81218-145">String</span></span>|<span data-ttu-id="81218-146">URL de ponto de extremidade de configuração a ser usada para registro</span><span class="sxs-lookup"><span data-stu-id="81218-146">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="81218-147">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="81218-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="81218-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="81218-148">Boolean</span></span>|<span data-ttu-id="81218-149">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="81218-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="81218-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="81218-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="81218-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="81218-151">Boolean</span></span>|<span data-ttu-id="81218-152">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados</span><span class="sxs-lookup"><span data-stu-id="81218-152">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="81218-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="81218-153">Response</span></span>
<span data-ttu-id="81218-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81218-154">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81218-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81218-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="81218-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81218-156">Request</span></span>
<span data-ttu-id="81218-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81218-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="81218-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="81218-158">Response</span></span>
<span data-ttu-id="81218-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81218-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





