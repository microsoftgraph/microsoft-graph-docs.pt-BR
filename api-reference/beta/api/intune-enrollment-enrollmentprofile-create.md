---
title: Criar enrollmentProfile
description: Crie um novo objeto de enrollmentProfile.
ms.openlocfilehash: 8b24964413250e9a0f9d8d98577e930e1ef99b84
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037448"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="8b2d7-103">Criar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="8b2d7-103">Create enrollmentProfile</span></span>

> <span data-ttu-id="8b2d7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8b2d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b2d7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8b2d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b2d7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8b2d7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b2d7-107">Crie um novo objeto de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8b2d7-107">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8b2d7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8b2d7-108">Prerequisites</span></span>
<span data-ttu-id="8b2d7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b2d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b2d7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b2d7-111">Permission type</span></span>|<span data-ttu-id="8b2d7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8b2d7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b2d7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b2d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b2d7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b2d7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8b2d7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b2d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b2d7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b2d7-116">Not supported.</span></span>|
|<span data-ttu-id="8b2d7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b2d7-117">Application</span></span>|<span data-ttu-id="8b2d7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b2d7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b2d7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b2d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="8b2d7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b2d7-120">Request headers</span></span>
|<span data-ttu-id="8b2d7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8b2d7-121">Header</span></span>|<span data-ttu-id="8b2d7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8b2d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b2d7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b2d7-123">Authorization</span></span>|<span data-ttu-id="8b2d7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b2d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b2d7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8b2d7-125">Accept</span></span>|<span data-ttu-id="8b2d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b2d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b2d7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b2d7-127">Request body</span></span>
<span data-ttu-id="8b2d7-128">No corpo da solicitação, fornece uma representação JSON para o objeto enrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="8b2d7-128">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="8b2d7-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o enrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="8b2d7-129">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="8b2d7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b2d7-130">Property</span></span>|<span data-ttu-id="8b2d7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b2d7-131">Type</span></span>|<span data-ttu-id="8b2d7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b2d7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b2d7-133">id</span><span class="sxs-lookup"><span data-stu-id="8b2d7-133">id</span></span>|<span data-ttu-id="8b2d7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b2d7-134">String</span></span>|<span data-ttu-id="8b2d7-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="8b2d7-135">The GUID for the object</span></span>|
|<span data-ttu-id="8b2d7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8b2d7-136">displayName</span></span>|<span data-ttu-id="8b2d7-137">String</span><span class="sxs-lookup"><span data-stu-id="8b2d7-137">String</span></span>|<span data-ttu-id="8b2d7-138">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="8b2d7-138">Name of the profile</span></span>|
|<span data-ttu-id="8b2d7-139">description</span><span class="sxs-lookup"><span data-stu-id="8b2d7-139">description</span></span>|<span data-ttu-id="8b2d7-140">String</span><span class="sxs-lookup"><span data-stu-id="8b2d7-140">String</span></span>|<span data-ttu-id="8b2d7-141">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="8b2d7-141">Description of the profile</span></span>|
|<span data-ttu-id="8b2d7-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="8b2d7-142">requiresUserAuthentication</span></span>|<span data-ttu-id="8b2d7-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="8b2d7-143">Boolean</span></span>|<span data-ttu-id="8b2d7-144">Indica se o perfil exige autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="8b2d7-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="8b2d7-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="8b2d7-145">configurationEndpointUrl</span></span>|<span data-ttu-id="8b2d7-146">String</span><span class="sxs-lookup"><span data-stu-id="8b2d7-146">String</span></span>|<span data-ttu-id="8b2d7-147">Url de ponto de extremidade de configuração a ser usado para registro</span><span class="sxs-lookup"><span data-stu-id="8b2d7-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="8b2d7-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="8b2d7-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="8b2d7-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="8b2d7-149">Boolean</span></span>|<span data-ttu-id="8b2d7-150">Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="8b2d7-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="8b2d7-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b2d7-151">Response</span></span>
<span data-ttu-id="8b2d7-152">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b2d7-152">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b2d7-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b2d7-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="8b2d7-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b2d7-154">Request</span></span>
<span data-ttu-id="8b2d7-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b2d7-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```

### <a name="response"></a><span data-ttu-id="8b2d7-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b2d7-156">Response</span></span>
<span data-ttu-id="8b2d7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8b2d7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```





