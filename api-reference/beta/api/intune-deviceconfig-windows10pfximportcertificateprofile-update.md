---
title: Atualizar windows10PFXImportCertificateProfile
description: Atualize as propriedades de um objeto windows10PFXImportCertificateProfile.
author: tfitzmac
ms.openlocfilehash: d5bc43583050bd0f48167360f360c656b0860a5e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302699"
---
# <a name="update-windows10pfximportcertificateprofile"></a><span data-ttu-id="ad089-103">Atualizar windows10PFXImportCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ad089-103">Update windows10PFXImportCertificateProfile</span></span>

> <span data-ttu-id="ad089-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ad089-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad089-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ad089-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad089-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ad089-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad089-107">Atualize as propriedades de um objeto [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ad089-107">Update the properties of a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad089-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ad089-108">Prerequisites</span></span>
<span data-ttu-id="ad089-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad089-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad089-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad089-111">Permission type</span></span>|<span data-ttu-id="ad089-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ad089-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad089-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad089-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad089-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad089-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ad089-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad089-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad089-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad089-116">Not supported.</span></span>|
|<span data-ttu-id="ad089-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad089-117">Application</span></span>|<span data-ttu-id="ad089-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad089-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad089-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad089-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ad089-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad089-120">Request headers</span></span>
|<span data-ttu-id="ad089-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad089-121">Header</span></span>|<span data-ttu-id="ad089-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ad089-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad089-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad089-123">Authorization</span></span>|<span data-ttu-id="ad089-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad089-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad089-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad089-125">Accept</span></span>|<span data-ttu-id="ad089-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad089-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad089-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad089-127">Request body</span></span>
<span data-ttu-id="ad089-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ad089-128">In the request body, supply a JSON representation for the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

<span data-ttu-id="ad089-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="ad089-129">The following table shows the properties that are required when you create the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span></span>

|<span data-ttu-id="ad089-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad089-130">Property</span></span>|<span data-ttu-id="ad089-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad089-131">Type</span></span>|<span data-ttu-id="ad089-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad089-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad089-133">id</span><span class="sxs-lookup"><span data-stu-id="ad089-133">id</span></span>|<span data-ttu-id="ad089-134">String</span><span class="sxs-lookup"><span data-stu-id="ad089-134">String</span></span>|<span data-ttu-id="ad089-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ad089-135">Key of the entity.</span></span> <span data-ttu-id="ad089-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad089-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad089-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad089-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ad089-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad089-138">DateTimeOffset</span></span>|<span data-ttu-id="ad089-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ad089-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ad089-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad089-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad089-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ad089-141">roleScopeTagIds</span></span>|<span data-ttu-id="ad089-142">String collection</span><span class="sxs-lookup"><span data-stu-id="ad089-142">String collection</span></span>|<span data-ttu-id="ad089-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="ad089-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ad089-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad089-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad089-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ad089-145">supportsScopeTags</span></span>|<span data-ttu-id="ad089-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad089-146">Boolean</span></span>|<span data-ttu-id="ad089-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ad089-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ad089-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ad089-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ad089-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="ad089-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ad089-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad089-150">This property is read-only.</span></span> <span data-ttu-id="ad089-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad089-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad089-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad089-152">createdDateTime</span></span>|<span data-ttu-id="ad089-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad089-153">DateTimeOffset</span></span>|<span data-ttu-id="ad089-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ad089-154">DateTime the object was created.</span></span> <span data-ttu-id="ad089-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad089-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad089-156">description</span><span class="sxs-lookup"><span data-stu-id="ad089-156">description</span></span>|<span data-ttu-id="ad089-157">String</span><span class="sxs-lookup"><span data-stu-id="ad089-157">String</span></span>|<span data-ttu-id="ad089-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ad089-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ad089-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad089-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad089-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ad089-160">displayName</span></span>|<span data-ttu-id="ad089-161">String</span><span class="sxs-lookup"><span data-stu-id="ad089-161">String</span></span>|<span data-ttu-id="ad089-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ad089-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ad089-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad089-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad089-164">version</span><span class="sxs-lookup"><span data-stu-id="ad089-164">version</span></span>|<span data-ttu-id="ad089-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ad089-165">Int32</span></span>|<span data-ttu-id="ad089-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ad089-166">Version of the device configuration.</span></span> <span data-ttu-id="ad089-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad089-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad089-168">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="ad089-168">keyStorageProvider</span></span>|[<span data-ttu-id="ad089-169">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="ad089-169">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="ad089-170">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="ad089-170">Not yet documented.</span></span> <span data-ttu-id="ad089-171">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="ad089-171">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="ad089-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad089-172">Response</span></span>
<span data-ttu-id="ad089-173">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad089-173">If successful, this method returns a `200 OK` response code and an updated [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad089-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad089-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad089-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad089-175">Request</span></span>
<span data-ttu-id="ad089-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad089-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 306

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```

### <a name="response"></a><span data-ttu-id="ad089-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad089-177">Response</span></span>
<span data-ttu-id="ad089-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad089-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "id": "4244277a-277a-4244-7a27-44427a274442",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```





