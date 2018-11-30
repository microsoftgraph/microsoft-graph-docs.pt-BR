---
title: Atualizar enrollmentProfile
description: Atualize as propriedades de um objeto enrollmentProfile.
ms.openlocfilehash: 6d8d0b6650c1094f1d2c46ab197eeb1781e097d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038983"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="55484-103">Atualizar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="55484-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="55484-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="55484-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55484-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="55484-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55484-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="55484-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55484-107">Atualize as propriedades de um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="55484-107">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="55484-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55484-108">Prerequisites</span></span>
<span data-ttu-id="55484-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55484-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55484-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55484-111">Permission type</span></span>|<span data-ttu-id="55484-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55484-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55484-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55484-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55484-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55484-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="55484-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55484-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55484-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55484-116">Not supported.</span></span>|
|<span data-ttu-id="55484-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55484-117">Application</span></span>|<span data-ttu-id="55484-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55484-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55484-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55484-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="55484-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55484-120">Request headers</span></span>
|<span data-ttu-id="55484-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55484-121">Header</span></span>|<span data-ttu-id="55484-122">Valor</span><span class="sxs-lookup"><span data-stu-id="55484-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55484-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="55484-123">Authorization</span></span>|<span data-ttu-id="55484-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55484-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55484-125">Accept</span><span class="sxs-lookup"><span data-stu-id="55484-125">Accept</span></span>|<span data-ttu-id="55484-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55484-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55484-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55484-127">Request body</span></span>
<span data-ttu-id="55484-128">No corpo da solicitação, fornece uma representação JSON para o objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="55484-128">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="55484-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="55484-129">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="55484-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55484-130">Property</span></span>|<span data-ttu-id="55484-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="55484-131">Type</span></span>|<span data-ttu-id="55484-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="55484-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55484-133">id</span><span class="sxs-lookup"><span data-stu-id="55484-133">id</span></span>|<span data-ttu-id="55484-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55484-134">String</span></span>|<span data-ttu-id="55484-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="55484-135">The GUID for the object</span></span>|
|<span data-ttu-id="55484-136">displayName</span><span class="sxs-lookup"><span data-stu-id="55484-136">displayName</span></span>|<span data-ttu-id="55484-137">String</span><span class="sxs-lookup"><span data-stu-id="55484-137">String</span></span>|<span data-ttu-id="55484-138">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="55484-138">Name of the profile</span></span>|
|<span data-ttu-id="55484-139">description</span><span class="sxs-lookup"><span data-stu-id="55484-139">description</span></span>|<span data-ttu-id="55484-140">String</span><span class="sxs-lookup"><span data-stu-id="55484-140">String</span></span>|<span data-ttu-id="55484-141">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="55484-141">Description of the profile</span></span>|
|<span data-ttu-id="55484-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="55484-142">requiresUserAuthentication</span></span>|<span data-ttu-id="55484-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="55484-143">Boolean</span></span>|<span data-ttu-id="55484-144">Indica se o perfil exige autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="55484-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="55484-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="55484-145">configurationEndpointUrl</span></span>|<span data-ttu-id="55484-146">String</span><span class="sxs-lookup"><span data-stu-id="55484-146">String</span></span>|<span data-ttu-id="55484-147">Url de ponto de extremidade de configuração a ser usado para registro</span><span class="sxs-lookup"><span data-stu-id="55484-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="55484-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="55484-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="55484-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="55484-149">Boolean</span></span>|<span data-ttu-id="55484-150">Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="55484-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="55484-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="55484-151">Response</span></span>
<span data-ttu-id="55484-152">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55484-152">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55484-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55484-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="55484-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55484-154">Request</span></span>
<span data-ttu-id="55484-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55484-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 250

{
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```

### <a name="response"></a><span data-ttu-id="55484-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="55484-156">Response</span></span>
<span data-ttu-id="55484-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55484-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





