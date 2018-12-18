---
title: Criar enrollmentProfile
description: Crie um novo objeto de enrollmentProfile.
author: tfitzmac
ms.openlocfilehash: becfc040bb7fa500a5378f16f50f6bcb2e4f106d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313647"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="a5b0e-103">Criar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a5b0e-103">Create enrollmentProfile</span></span>

> <span data-ttu-id="a5b0e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a5b0e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5b0e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a5b0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5b0e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a5b0e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5b0e-107">Crie um novo objeto de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a5b0e-107">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a5b0e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a5b0e-108">Prerequisites</span></span>
<span data-ttu-id="a5b0e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5b0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5b0e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5b0e-111">Permission type</span></span>|<span data-ttu-id="a5b0e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a5b0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5b0e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5b0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5b0e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5b0e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a5b0e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5b0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5b0e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5b0e-116">Not supported.</span></span>|
|<span data-ttu-id="a5b0e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5b0e-117">Application</span></span>|<span data-ttu-id="a5b0e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5b0e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5b0e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5b0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="a5b0e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5b0e-120">Request headers</span></span>
|<span data-ttu-id="a5b0e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5b0e-121">Header</span></span>|<span data-ttu-id="a5b0e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a5b0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5b0e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5b0e-123">Authorization</span></span>|<span data-ttu-id="a5b0e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5b0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5b0e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a5b0e-125">Accept</span></span>|<span data-ttu-id="a5b0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5b0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5b0e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5b0e-127">Request body</span></span>
<span data-ttu-id="a5b0e-128">No corpo da solicitação, fornece uma representação JSON para o objeto enrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="a5b0e-128">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="a5b0e-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o enrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="a5b0e-129">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="a5b0e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5b0e-130">Property</span></span>|<span data-ttu-id="a5b0e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5b0e-131">Type</span></span>|<span data-ttu-id="a5b0e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5b0e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5b0e-133">id</span><span class="sxs-lookup"><span data-stu-id="a5b0e-133">id</span></span>|<span data-ttu-id="a5b0e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5b0e-134">String</span></span>|<span data-ttu-id="a5b0e-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="a5b0e-135">The GUID for the object</span></span>|
|<span data-ttu-id="a5b0e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a5b0e-136">displayName</span></span>|<span data-ttu-id="a5b0e-137">String</span><span class="sxs-lookup"><span data-stu-id="a5b0e-137">String</span></span>|<span data-ttu-id="a5b0e-138">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="a5b0e-138">Name of the profile</span></span>|
|<span data-ttu-id="a5b0e-139">description</span><span class="sxs-lookup"><span data-stu-id="a5b0e-139">description</span></span>|<span data-ttu-id="a5b0e-140">String</span><span class="sxs-lookup"><span data-stu-id="a5b0e-140">String</span></span>|<span data-ttu-id="a5b0e-141">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="a5b0e-141">Description of the profile</span></span>|
|<span data-ttu-id="a5b0e-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="a5b0e-142">requiresUserAuthentication</span></span>|<span data-ttu-id="a5b0e-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5b0e-143">Boolean</span></span>|<span data-ttu-id="a5b0e-144">Indica se o perfil exige autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="a5b0e-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="a5b0e-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="a5b0e-145">configurationEndpointUrl</span></span>|<span data-ttu-id="a5b0e-146">String</span><span class="sxs-lookup"><span data-stu-id="a5b0e-146">String</span></span>|<span data-ttu-id="a5b0e-147">Url de ponto de extremidade de configuração a ser usado para registro</span><span class="sxs-lookup"><span data-stu-id="a5b0e-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="a5b0e-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="a5b0e-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="a5b0e-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5b0e-149">Boolean</span></span>|<span data-ttu-id="a5b0e-150">Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="a5b0e-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="a5b0e-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5b0e-151">Response</span></span>
<span data-ttu-id="a5b0e-152">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5b0e-152">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5b0e-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5b0e-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5b0e-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5b0e-154">Request</span></span>
<span data-ttu-id="a5b0e-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5b0e-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a5b0e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5b0e-156">Response</span></span>
<span data-ttu-id="a5b0e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5b0e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





