---
title: Atualizar windows10SecureAssessmentConfiguration
description: Atualizar as propriedades de um objeto windows10SecureAssessmentConfiguration.
author: tfitzmac
ms.openlocfilehash: 903a5f16f35456aecc6285f87f371a73ebee25ae
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304988"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="1ed24-103">Atualizar windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ed24-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="1ed24-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1ed24-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ed24-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1ed24-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ed24-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1ed24-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ed24-107">Atualizar as propriedades de um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ed24-107">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ed24-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ed24-108">Prerequisites</span></span>
<span data-ttu-id="1ed24-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ed24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ed24-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ed24-111">Permission type</span></span>|<span data-ttu-id="1ed24-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ed24-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ed24-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ed24-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ed24-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ed24-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ed24-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ed24-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ed24-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ed24-116">Not supported.</span></span>|
|<span data-ttu-id="1ed24-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ed24-117">Application</span></span>|<span data-ttu-id="1ed24-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ed24-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ed24-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ed24-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1ed24-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ed24-120">Request headers</span></span>
|<span data-ttu-id="1ed24-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ed24-121">Header</span></span>|<span data-ttu-id="1ed24-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1ed24-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ed24-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ed24-123">Authorization</span></span>|<span data-ttu-id="1ed24-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ed24-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ed24-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1ed24-125">Accept</span></span>|<span data-ttu-id="1ed24-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ed24-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ed24-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ed24-127">Request body</span></span>
<span data-ttu-id="1ed24-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ed24-128">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="1ed24-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ed24-129">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="1ed24-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ed24-130">Property</span></span>|<span data-ttu-id="1ed24-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ed24-131">Type</span></span>|<span data-ttu-id="1ed24-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ed24-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ed24-133">id</span><span class="sxs-lookup"><span data-stu-id="1ed24-133">id</span></span>|<span data-ttu-id="1ed24-134">String</span><span class="sxs-lookup"><span data-stu-id="1ed24-134">String</span></span>|<span data-ttu-id="1ed24-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1ed24-135">Key of the entity.</span></span> <span data-ttu-id="1ed24-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ed24-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ed24-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ed24-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1ed24-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ed24-138">DateTimeOffset</span></span>|<span data-ttu-id="1ed24-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1ed24-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1ed24-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ed24-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ed24-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1ed24-141">roleScopeTagIds</span></span>|<span data-ttu-id="1ed24-142">String collection</span><span class="sxs-lookup"><span data-stu-id="1ed24-142">String collection</span></span>|<span data-ttu-id="1ed24-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="1ed24-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1ed24-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ed24-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ed24-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1ed24-145">supportsScopeTags</span></span>|<span data-ttu-id="1ed24-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ed24-146">Boolean</span></span>|<span data-ttu-id="1ed24-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="1ed24-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1ed24-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="1ed24-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1ed24-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="1ed24-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1ed24-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ed24-150">This property is read-only.</span></span> <span data-ttu-id="1ed24-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ed24-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ed24-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ed24-152">createdDateTime</span></span>|<span data-ttu-id="1ed24-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ed24-153">DateTimeOffset</span></span>|<span data-ttu-id="1ed24-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1ed24-154">DateTime the object was created.</span></span> <span data-ttu-id="1ed24-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ed24-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ed24-156">description</span><span class="sxs-lookup"><span data-stu-id="1ed24-156">description</span></span>|<span data-ttu-id="1ed24-157">String</span><span class="sxs-lookup"><span data-stu-id="1ed24-157">String</span></span>|<span data-ttu-id="1ed24-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1ed24-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1ed24-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ed24-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ed24-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1ed24-160">displayName</span></span>|<span data-ttu-id="1ed24-161">String</span><span class="sxs-lookup"><span data-stu-id="1ed24-161">String</span></span>|<span data-ttu-id="1ed24-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1ed24-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1ed24-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ed24-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ed24-164">version</span><span class="sxs-lookup"><span data-stu-id="1ed24-164">version</span></span>|<span data-ttu-id="1ed24-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1ed24-165">Int32</span></span>|<span data-ttu-id="1ed24-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1ed24-166">Version of the device configuration.</span></span> <span data-ttu-id="1ed24-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ed24-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ed24-168">launchUri</span><span class="sxs-lookup"><span data-stu-id="1ed24-168">launchUri</span></span>|<span data-ttu-id="1ed24-169">String</span><span class="sxs-lookup"><span data-stu-id="1ed24-169">String</span></span>|<span data-ttu-id="1ed24-170">Link da URL para uma avaliação que é carregada automaticamente quando o navegador de avaliação segura é iniciado.</span><span class="sxs-lookup"><span data-stu-id="1ed24-170">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="1ed24-171">Ele precisa ser uma URL válida (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="1ed24-171">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="1ed24-172">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="1ed24-172">configurationAccount</span></span>|<span data-ttu-id="1ed24-173">String</span><span class="sxs-lookup"><span data-stu-id="1ed24-173">String</span></span>|<span data-ttu-id="1ed24-174">A conta usada para configurar o dispositivo Windows para realizar o teste.</span><span class="sxs-lookup"><span data-stu-id="1ed24-174">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="1ed24-175">O usuário pode ser uma conta de domínio (domínio\usuário), uma conta do AAD (nomedeusuário@locatário.com) ou uma conta local (nomedeusuário).</span><span class="sxs-lookup"><span data-stu-id="1ed24-175">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="1ed24-176">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="1ed24-176">configurationAccountType</span></span>|[<span data-ttu-id="1ed24-177">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="1ed24-177">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="1ed24-178">O tipo de conta usado para por ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="1ed24-178">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="1ed24-179">Os valores possíveis são: `azureADAccount`, `domainAccount`, `localAccount`.</span><span class="sxs-lookup"><span data-stu-id="1ed24-179">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="1ed24-180">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="1ed24-180">allowPrinting</span></span>|<span data-ttu-id="1ed24-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ed24-181">Boolean</span></span>|<span data-ttu-id="1ed24-182">Indica se o aplicativo deve ou não ter permissão de impressão durante o teste.</span><span class="sxs-lookup"><span data-stu-id="1ed24-182">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="1ed24-183">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="1ed24-183">allowScreenCapture</span></span>|<span data-ttu-id="1ed24-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ed24-184">Boolean</span></span>|<span data-ttu-id="1ed24-185">Indica se a capacidade de captura de tela deve ou não ser permitida durante um teste.</span><span class="sxs-lookup"><span data-stu-id="1ed24-185">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="1ed24-186">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="1ed24-186">allowTextSuggestion</span></span>|<span data-ttu-id="1ed24-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ed24-187">Boolean</span></span>|<span data-ttu-id="1ed24-188">Indica se sugestões de texto devem ou não ser permitidas durante o teste.</span><span class="sxs-lookup"><span data-stu-id="1ed24-188">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="1ed24-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ed24-189">Response</span></span>
<span data-ttu-id="1ed24-190">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ed24-190">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ed24-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ed24-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ed24-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ed24-192">Request</span></span>
<span data-ttu-id="1ed24-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ed24-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 486

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="1ed24-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ed24-194">Response</span></span>
<span data-ttu-id="1ed24-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ed24-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```





