---
title: Criar defaultDeviceCompliancePolicy
description: Crie um novo objeto de defaultDeviceCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 79911794adf153a18b7af7f58cec72baf56f3015
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964421"
---
# <a name="create-defaultdevicecompliancepolicy"></a><span data-ttu-id="d6fd6-103">Criar defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d6fd6-103">Create defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="d6fd6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6fd6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6fd6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6fd6-107">Crie um novo objeto de [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="d6fd6-107">Create a new [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d6fd6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6fd6-108">Prerequisites</span></span>
<span data-ttu-id="d6fd6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6fd6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6fd6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6fd6-111">Permission type</span></span>|<span data-ttu-id="d6fd6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6fd6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6fd6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6fd6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6fd6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6fd6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6fd6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6fd6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6fd6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-116">Not supported.</span></span>|
|<span data-ttu-id="d6fd6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6fd6-117">Application</span></span>|<span data-ttu-id="d6fd6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6fd6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6fd6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="d6fd6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6fd6-120">Request headers</span></span>
|<span data-ttu-id="d6fd6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6fd6-121">Header</span></span>|<span data-ttu-id="d6fd6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d6fd6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6fd6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6fd6-123">Authorization</span></span>|<span data-ttu-id="d6fd6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6fd6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6fd6-125">Accept</span></span>|<span data-ttu-id="d6fd6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6fd6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6fd6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6fd6-127">Request body</span></span>
<span data-ttu-id="d6fd6-128">No corpo da solicitação, fornece uma representação JSON para o objeto defaultDeviceCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-128">In the request body, supply a JSON representation for the defaultDeviceCompliancePolicy object.</span></span>

<span data-ttu-id="d6fd6-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o defaultDeviceCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-129">The following table shows the properties that are required when you create the defaultDeviceCompliancePolicy.</span></span>

|<span data-ttu-id="d6fd6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6fd6-130">Property</span></span>|<span data-ttu-id="d6fd6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6fd6-131">Type</span></span>|<span data-ttu-id="d6fd6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6fd6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6fd6-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d6fd6-133">roleScopeTagIds</span></span>|<span data-ttu-id="d6fd6-134">String collection</span><span class="sxs-lookup"><span data-stu-id="d6fd6-134">String collection</span></span>|<span data-ttu-id="d6fd6-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d6fd6-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d6fd6-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d6fd6-137">id</span><span class="sxs-lookup"><span data-stu-id="d6fd6-137">id</span></span>|<span data-ttu-id="d6fd6-138">String</span><span class="sxs-lookup"><span data-stu-id="d6fd6-138">String</span></span>|<span data-ttu-id="d6fd6-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-139">Key of the entity.</span></span> <span data-ttu-id="d6fd6-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d6fd6-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d6fd6-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6fd6-141">createdDateTime</span></span>|<span data-ttu-id="d6fd6-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6fd6-142">DateTimeOffset</span></span>|<span data-ttu-id="d6fd6-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-143">DateTime the object was created.</span></span> <span data-ttu-id="d6fd6-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d6fd6-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d6fd6-145">description</span><span class="sxs-lookup"><span data-stu-id="d6fd6-145">description</span></span>|<span data-ttu-id="d6fd6-146">String</span><span class="sxs-lookup"><span data-stu-id="d6fd6-146">String</span></span>|<span data-ttu-id="d6fd6-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d6fd6-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d6fd6-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d6fd6-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6fd6-149">lastModifiedDateTime</span></span>|<span data-ttu-id="d6fd6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6fd6-150">DateTimeOffset</span></span>|<span data-ttu-id="d6fd6-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-151">DateTime the object was last modified.</span></span> <span data-ttu-id="d6fd6-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d6fd6-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d6fd6-153">displayName</span><span class="sxs-lookup"><span data-stu-id="d6fd6-153">displayName</span></span>|<span data-ttu-id="d6fd6-154">String</span><span class="sxs-lookup"><span data-stu-id="d6fd6-154">String</span></span>|<span data-ttu-id="d6fd6-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d6fd6-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d6fd6-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d6fd6-157">version</span><span class="sxs-lookup"><span data-stu-id="d6fd6-157">version</span></span>|<span data-ttu-id="d6fd6-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d6fd6-158">Int32</span></span>|<span data-ttu-id="d6fd6-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-159">Version of the device configuration.</span></span> <span data-ttu-id="d6fd6-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d6fd6-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d6fd6-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6fd6-161">Response</span></span>
<span data-ttu-id="d6fd6-162">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-162">If successful, this method returns a `201 Created` response code and a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6fd6-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6fd6-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="d6fd6-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6fd6-164">Request</span></span>
<span data-ttu-id="d6fd6-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 293

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="d6fd6-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6fd6-166">Response</span></span>
<span data-ttu-id="d6fd6-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6fd6-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 401

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "a285f027-f027-a285-27f0-85a227f085a2",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```





