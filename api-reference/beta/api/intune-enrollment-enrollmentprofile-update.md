---
title: Atualizar enrollmentProfile
description: Atualize as propriedades de um objeto enrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 85cceaaaaa66822340539c38f6ab8ecde88eae1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400736"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="ce132-103">Atualizar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ce132-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="ce132-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ce132-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ce132-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ce132-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce132-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ce132-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce132-107">Atualize as propriedades de um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ce132-107">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce132-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ce132-108">Prerequisites</span></span>
<span data-ttu-id="ce132-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce132-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ce132-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce132-111">Permission type</span></span>|<span data-ttu-id="ce132-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ce132-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce132-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce132-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce132-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce132-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ce132-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce132-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce132-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce132-116">Not supported.</span></span>|
|<span data-ttu-id="ce132-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce132-117">Application</span></span>|<span data-ttu-id="ce132-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce132-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce132-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce132-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="ce132-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce132-120">Request headers</span></span>
|<span data-ttu-id="ce132-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ce132-121">Header</span></span>|<span data-ttu-id="ce132-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ce132-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce132-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce132-123">Authorization</span></span>|<span data-ttu-id="ce132-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce132-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce132-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ce132-125">Accept</span></span>|<span data-ttu-id="ce132-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce132-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce132-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce132-127">Request body</span></span>
<span data-ttu-id="ce132-128">No corpo da solicitação, fornece uma representação JSON para o objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ce132-128">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="ce132-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="ce132-129">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="ce132-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce132-130">Property</span></span>|<span data-ttu-id="ce132-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce132-131">Type</span></span>|<span data-ttu-id="ce132-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce132-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce132-133">id</span><span class="sxs-lookup"><span data-stu-id="ce132-133">id</span></span>|<span data-ttu-id="ce132-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce132-134">String</span></span>|<span data-ttu-id="ce132-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="ce132-135">The GUID for the object</span></span>|
|<span data-ttu-id="ce132-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ce132-136">displayName</span></span>|<span data-ttu-id="ce132-137">String</span><span class="sxs-lookup"><span data-stu-id="ce132-137">String</span></span>|<span data-ttu-id="ce132-138">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="ce132-138">Name of the profile</span></span>|
|<span data-ttu-id="ce132-139">description</span><span class="sxs-lookup"><span data-stu-id="ce132-139">description</span></span>|<span data-ttu-id="ce132-140">String</span><span class="sxs-lookup"><span data-stu-id="ce132-140">String</span></span>|<span data-ttu-id="ce132-141">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="ce132-141">Description of the profile</span></span>|
|<span data-ttu-id="ce132-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="ce132-142">requiresUserAuthentication</span></span>|<span data-ttu-id="ce132-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce132-143">Boolean</span></span>|<span data-ttu-id="ce132-144">Indica se o perfil exige autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="ce132-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="ce132-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="ce132-145">configurationEndpointUrl</span></span>|<span data-ttu-id="ce132-146">String</span><span class="sxs-lookup"><span data-stu-id="ce132-146">String</span></span>|<span data-ttu-id="ce132-147">Url de ponto de extremidade de configuração a ser usado para registro</span><span class="sxs-lookup"><span data-stu-id="ce132-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="ce132-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="ce132-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="ce132-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce132-149">Boolean</span></span>|<span data-ttu-id="ce132-150">Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="ce132-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="ce132-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="ce132-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="ce132-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce132-152">Boolean</span></span>|<span data-ttu-id="ce132-153">Indica que o Portal da empresa é necessária em dispositivos de inscritos do Assistente de instalação</span><span class="sxs-lookup"><span data-stu-id="ce132-153">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="ce132-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce132-154">Response</span></span>
<span data-ttu-id="ce132-155">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce132-155">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce132-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce132-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce132-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce132-157">Request</span></span>
<span data-ttu-id="ce132-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce132-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ce132-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce132-159">Response</span></span>
<span data-ttu-id="ce132-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce132-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




