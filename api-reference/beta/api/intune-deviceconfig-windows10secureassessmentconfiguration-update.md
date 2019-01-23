---
title: Atualizar windows10SecureAssessmentConfiguration
description: Atualizar as propriedades de um objeto windows10SecureAssessmentConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4503276def73977eb623eb472b7dd9fcf1446e6f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421407"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="dce6e-103">Atualizar windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="dce6e-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="dce6e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="dce6e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dce6e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dce6e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dce6e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="dce6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dce6e-107">Atualizar as propriedades de um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dce6e-107">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dce6e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dce6e-108">Prerequisites</span></span>
<span data-ttu-id="dce6e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dce6e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dce6e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dce6e-111">Permission type</span></span>|<span data-ttu-id="dce6e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dce6e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dce6e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dce6e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dce6e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dce6e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dce6e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dce6e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dce6e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dce6e-116">Not supported.</span></span>|
|<span data-ttu-id="dce6e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dce6e-117">Application</span></span>|<span data-ttu-id="dce6e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dce6e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dce6e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dce6e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dce6e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dce6e-120">Request headers</span></span>
|<span data-ttu-id="dce6e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dce6e-121">Header</span></span>|<span data-ttu-id="dce6e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dce6e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dce6e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dce6e-123">Authorization</span></span>|<span data-ttu-id="dce6e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dce6e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dce6e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dce6e-125">Accept</span></span>|<span data-ttu-id="dce6e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dce6e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dce6e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dce6e-127">Request body</span></span>
<span data-ttu-id="dce6e-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dce6e-128">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="dce6e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dce6e-129">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="dce6e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dce6e-130">Property</span></span>|<span data-ttu-id="dce6e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dce6e-131">Type</span></span>|<span data-ttu-id="dce6e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dce6e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dce6e-133">id</span><span class="sxs-lookup"><span data-stu-id="dce6e-133">id</span></span>|<span data-ttu-id="dce6e-134">String</span><span class="sxs-lookup"><span data-stu-id="dce6e-134">String</span></span>|<span data-ttu-id="dce6e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dce6e-135">Key of the entity.</span></span> <span data-ttu-id="dce6e-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dce6e-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dce6e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dce6e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="dce6e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dce6e-138">DateTimeOffset</span></span>|<span data-ttu-id="dce6e-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="dce6e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="dce6e-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dce6e-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dce6e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dce6e-141">roleScopeTagIds</span></span>|<span data-ttu-id="dce6e-142">String collection</span><span class="sxs-lookup"><span data-stu-id="dce6e-142">String collection</span></span>|<span data-ttu-id="dce6e-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="dce6e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dce6e-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dce6e-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dce6e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="dce6e-145">supportsScopeTags</span></span>|<span data-ttu-id="dce6e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="dce6e-146">Boolean</span></span>|<span data-ttu-id="dce6e-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="dce6e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dce6e-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="dce6e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dce6e-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="dce6e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dce6e-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dce6e-150">This property is read-only.</span></span> <span data-ttu-id="dce6e-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dce6e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dce6e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dce6e-152">createdDateTime</span></span>|<span data-ttu-id="dce6e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dce6e-153">DateTimeOffset</span></span>|<span data-ttu-id="dce6e-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="dce6e-154">DateTime the object was created.</span></span> <span data-ttu-id="dce6e-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dce6e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dce6e-156">description</span><span class="sxs-lookup"><span data-stu-id="dce6e-156">description</span></span>|<span data-ttu-id="dce6e-157">String</span><span class="sxs-lookup"><span data-stu-id="dce6e-157">String</span></span>|<span data-ttu-id="dce6e-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dce6e-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dce6e-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dce6e-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dce6e-160">displayName</span><span class="sxs-lookup"><span data-stu-id="dce6e-160">displayName</span></span>|<span data-ttu-id="dce6e-161">String</span><span class="sxs-lookup"><span data-stu-id="dce6e-161">String</span></span>|<span data-ttu-id="dce6e-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dce6e-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dce6e-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dce6e-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dce6e-164">version</span><span class="sxs-lookup"><span data-stu-id="dce6e-164">version</span></span>|<span data-ttu-id="dce6e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="dce6e-165">Int32</span></span>|<span data-ttu-id="dce6e-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dce6e-166">Version of the device configuration.</span></span> <span data-ttu-id="dce6e-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dce6e-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dce6e-168">launchUri</span><span class="sxs-lookup"><span data-stu-id="dce6e-168">launchUri</span></span>|<span data-ttu-id="dce6e-169">String</span><span class="sxs-lookup"><span data-stu-id="dce6e-169">String</span></span>|<span data-ttu-id="dce6e-170">Link da URL para uma avaliação que é carregada automaticamente quando o navegador de avaliação segura é iniciado.</span><span class="sxs-lookup"><span data-stu-id="dce6e-170">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="dce6e-171">Ele precisa ser uma URL válida (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="dce6e-171">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="dce6e-172">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="dce6e-172">configurationAccount</span></span>|<span data-ttu-id="dce6e-173">String</span><span class="sxs-lookup"><span data-stu-id="dce6e-173">String</span></span>|<span data-ttu-id="dce6e-174">A conta usada para configurar o dispositivo Windows para realizar o teste.</span><span class="sxs-lookup"><span data-stu-id="dce6e-174">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="dce6e-175">O usuário pode ser uma conta de domínio (domínio\usuário), uma conta do AAD (nomedeusuário@locatário.com) ou uma conta local (nomedeusuário).</span><span class="sxs-lookup"><span data-stu-id="dce6e-175">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="dce6e-176">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="dce6e-176">configurationAccountType</span></span>|[<span data-ttu-id="dce6e-177">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="dce6e-177">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="dce6e-178">O tipo de conta usado para por ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="dce6e-178">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="dce6e-179">Os valores possíveis são: `azureADAccount`, `domainAccount`, `localAccount`.</span><span class="sxs-lookup"><span data-stu-id="dce6e-179">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="dce6e-180">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="dce6e-180">allowPrinting</span></span>|<span data-ttu-id="dce6e-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="dce6e-181">Boolean</span></span>|<span data-ttu-id="dce6e-182">Indica se o aplicativo deve ou não ter permissão de impressão durante o teste.</span><span class="sxs-lookup"><span data-stu-id="dce6e-182">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="dce6e-183">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="dce6e-183">allowScreenCapture</span></span>|<span data-ttu-id="dce6e-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="dce6e-184">Boolean</span></span>|<span data-ttu-id="dce6e-185">Indica se a capacidade de captura de tela deve ou não ser permitida durante um teste.</span><span class="sxs-lookup"><span data-stu-id="dce6e-185">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="dce6e-186">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="dce6e-186">allowTextSuggestion</span></span>|<span data-ttu-id="dce6e-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="dce6e-187">Boolean</span></span>|<span data-ttu-id="dce6e-188">Indica se sugestões de texto devem ou não ser permitidas durante o teste.</span><span class="sxs-lookup"><span data-stu-id="dce6e-188">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="dce6e-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="dce6e-189">Response</span></span>
<span data-ttu-id="dce6e-190">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dce6e-190">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dce6e-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dce6e-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="dce6e-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dce6e-192">Request</span></span>
<span data-ttu-id="dce6e-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dce6e-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 499

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
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

### <a name="response"></a><span data-ttu-id="dce6e-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="dce6e-194">Response</span></span>
<span data-ttu-id="dce6e-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dce6e-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




