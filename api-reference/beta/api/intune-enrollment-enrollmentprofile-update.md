---
title: Atualizar enrollmentProfile
description: Atualiza as propriedades de um objeto enrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a3283a87f544050879cd2ba54a0dc47111239d0a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701988"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="d64c7-103">Atualizar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d64c7-103">Update enrollmentProfile</span></span>

<span data-ttu-id="d64c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d64c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d64c7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d64c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d64c7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d64c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d64c7-107">Atualiza as propriedades de um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d64c7-107">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d64c7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d64c7-108">Prerequisites</span></span>
<span data-ttu-id="d64c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d64c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d64c7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d64c7-111">Permission type</span></span>|<span data-ttu-id="d64c7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d64c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d64c7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d64c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d64c7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64c7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d64c7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d64c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d64c7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d64c7-116">Not supported.</span></span>|
|<span data-ttu-id="d64c7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d64c7-117">Application</span></span>|<span data-ttu-id="d64c7-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64c7-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d64c7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d64c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="d64c7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d64c7-120">Request headers</span></span>
|<span data-ttu-id="d64c7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d64c7-121">Header</span></span>|<span data-ttu-id="d64c7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d64c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d64c7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d64c7-123">Authorization</span></span>|<span data-ttu-id="d64c7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d64c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d64c7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d64c7-125">Accept</span></span>|<span data-ttu-id="d64c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d64c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d64c7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d64c7-127">Request body</span></span>
<span data-ttu-id="d64c7-128">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d64c7-128">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="d64c7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="d64c7-129">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="d64c7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d64c7-130">Property</span></span>|<span data-ttu-id="d64c7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d64c7-131">Type</span></span>|<span data-ttu-id="d64c7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d64c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d64c7-133">id</span><span class="sxs-lookup"><span data-stu-id="d64c7-133">id</span></span>|<span data-ttu-id="d64c7-134">String</span><span class="sxs-lookup"><span data-stu-id="d64c7-134">String</span></span>|<span data-ttu-id="d64c7-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="d64c7-135">The GUID for the object</span></span>|
|<span data-ttu-id="d64c7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d64c7-136">displayName</span></span>|<span data-ttu-id="d64c7-137">String</span><span class="sxs-lookup"><span data-stu-id="d64c7-137">String</span></span>|<span data-ttu-id="d64c7-138">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="d64c7-138">Name of the profile</span></span>|
|<span data-ttu-id="d64c7-139">description</span><span class="sxs-lookup"><span data-stu-id="d64c7-139">description</span></span>|<span data-ttu-id="d64c7-140">String</span><span class="sxs-lookup"><span data-stu-id="d64c7-140">String</span></span>|<span data-ttu-id="d64c7-141">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="d64c7-141">Description of the profile</span></span>|
|<span data-ttu-id="d64c7-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="d64c7-142">requiresUserAuthentication</span></span>|<span data-ttu-id="d64c7-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="d64c7-143">Boolean</span></span>|<span data-ttu-id="d64c7-144">Indica se o perfil requer autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="d64c7-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="d64c7-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="d64c7-145">configurationEndpointUrl</span></span>|<span data-ttu-id="d64c7-146">String</span><span class="sxs-lookup"><span data-stu-id="d64c7-146">String</span></span>|<span data-ttu-id="d64c7-147">URL de ponto de extremidade de configuração a ser usada para registro</span><span class="sxs-lookup"><span data-stu-id="d64c7-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="d64c7-148">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="d64c7-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="d64c7-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="d64c7-149">Boolean</span></span>|<span data-ttu-id="d64c7-150">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="d64c7-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="d64c7-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="d64c7-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="d64c7-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="d64c7-152">Boolean</span></span>|<span data-ttu-id="d64c7-153">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados</span><span class="sxs-lookup"><span data-stu-id="d64c7-153">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="d64c7-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d64c7-154">Response</span></span>
<span data-ttu-id="d64c7-155">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d64c7-155">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d64c7-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d64c7-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="d64c7-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d64c7-157">Request</span></span>
<span data-ttu-id="d64c7-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d64c7-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d64c7-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="d64c7-159">Response</span></span>
<span data-ttu-id="d64c7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d64c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





