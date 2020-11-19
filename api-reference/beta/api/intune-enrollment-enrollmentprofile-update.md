---
title: Atualizar enrollmentProfile
description: Atualiza as propriedades de um objeto enrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fdecd9a85e86cefa72659088d4ed3fe594eb2d94
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212612"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="d888e-103">Atualizar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d888e-103">Update enrollmentProfile</span></span>

<span data-ttu-id="d888e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d888e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d888e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d888e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d888e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d888e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d888e-107">Atualiza as propriedades de um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d888e-107">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d888e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d888e-108">Prerequisites</span></span>
<span data-ttu-id="d888e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d888e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d888e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d888e-111">Permission type</span></span>|<span data-ttu-id="d888e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d888e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d888e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d888e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d888e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d888e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d888e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d888e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d888e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d888e-116">Not supported.</span></span>|
|<span data-ttu-id="d888e-117">Application</span><span class="sxs-lookup"><span data-stu-id="d888e-117">Application</span></span>|<span data-ttu-id="d888e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d888e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d888e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d888e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="d888e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d888e-120">Request headers</span></span>
|<span data-ttu-id="d888e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d888e-121">Header</span></span>|<span data-ttu-id="d888e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d888e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d888e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d888e-123">Authorization</span></span>|<span data-ttu-id="d888e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d888e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d888e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d888e-125">Accept</span></span>|<span data-ttu-id="d888e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d888e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d888e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d888e-127">Request body</span></span>
<span data-ttu-id="d888e-128">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d888e-128">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="d888e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="d888e-129">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="d888e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d888e-130">Property</span></span>|<span data-ttu-id="d888e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d888e-131">Type</span></span>|<span data-ttu-id="d888e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d888e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d888e-133">id</span><span class="sxs-lookup"><span data-stu-id="d888e-133">id</span></span>|<span data-ttu-id="d888e-134">String</span><span class="sxs-lookup"><span data-stu-id="d888e-134">String</span></span>|<span data-ttu-id="d888e-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="d888e-135">The GUID for the object</span></span>|
|<span data-ttu-id="d888e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d888e-136">displayName</span></span>|<span data-ttu-id="d888e-137">String</span><span class="sxs-lookup"><span data-stu-id="d888e-137">String</span></span>|<span data-ttu-id="d888e-138">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="d888e-138">Name of the profile</span></span>|
|<span data-ttu-id="d888e-139">description</span><span class="sxs-lookup"><span data-stu-id="d888e-139">description</span></span>|<span data-ttu-id="d888e-140">String</span><span class="sxs-lookup"><span data-stu-id="d888e-140">String</span></span>|<span data-ttu-id="d888e-141">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="d888e-141">Description of the profile</span></span>|
|<span data-ttu-id="d888e-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="d888e-142">requiresUserAuthentication</span></span>|<span data-ttu-id="d888e-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="d888e-143">Boolean</span></span>|<span data-ttu-id="d888e-144">Indica se o perfil requer autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="d888e-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="d888e-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="d888e-145">configurationEndpointUrl</span></span>|<span data-ttu-id="d888e-146">String</span><span class="sxs-lookup"><span data-stu-id="d888e-146">String</span></span>|<span data-ttu-id="d888e-147">URL de ponto de extremidade de configuração a ser usada para registro</span><span class="sxs-lookup"><span data-stu-id="d888e-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="d888e-148">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="d888e-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="d888e-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="d888e-149">Boolean</span></span>|<span data-ttu-id="d888e-150">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="d888e-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="d888e-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="d888e-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="d888e-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="d888e-152">Boolean</span></span>|<span data-ttu-id="d888e-153">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados</span><span class="sxs-lookup"><span data-stu-id="d888e-153">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="d888e-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d888e-154">Response</span></span>
<span data-ttu-id="d888e-155">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d888e-155">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d888e-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d888e-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="d888e-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d888e-157">Request</span></span>
<span data-ttu-id="d888e-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d888e-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d888e-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="d888e-159">Response</span></span>
<span data-ttu-id="d888e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d888e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




