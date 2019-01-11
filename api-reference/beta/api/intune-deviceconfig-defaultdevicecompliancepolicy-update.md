---
title: Atualizar defaultDeviceCompliancePolicy
description: Atualize as propriedades de um objeto defaultDeviceCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a6bad561bc82777c594191a34eb6dec8b3a3e3ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817399"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="688e4-103">Atualizar defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="688e4-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="688e4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="688e4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="688e4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="688e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="688e4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="688e4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="688e4-107">Atualize as propriedades de um objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="688e4-107">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="688e4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="688e4-108">Prerequisites</span></span>
<span data-ttu-id="688e4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="688e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="688e4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="688e4-111">Permission type</span></span>|<span data-ttu-id="688e4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="688e4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="688e4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="688e4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="688e4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="688e4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="688e4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="688e4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="688e4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="688e4-116">Not supported.</span></span>|
|<span data-ttu-id="688e4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="688e4-117">Application</span></span>|<span data-ttu-id="688e4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="688e4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="688e4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="688e4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="688e4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="688e4-120">Request headers</span></span>
|<span data-ttu-id="688e4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="688e4-121">Header</span></span>|<span data-ttu-id="688e4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="688e4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="688e4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="688e4-123">Authorization</span></span>|<span data-ttu-id="688e4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="688e4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="688e4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="688e4-125">Accept</span></span>|<span data-ttu-id="688e4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="688e4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="688e4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="688e4-127">Request body</span></span>
<span data-ttu-id="688e4-128">No corpo da solicitação, fornece uma representação JSON para o objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="688e4-128">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="688e4-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="688e4-129">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="688e4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="688e4-130">Property</span></span>|<span data-ttu-id="688e4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="688e4-131">Type</span></span>|<span data-ttu-id="688e4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="688e4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="688e4-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="688e4-133">roleScopeTagIds</span></span>|<span data-ttu-id="688e4-134">String collection</span><span class="sxs-lookup"><span data-stu-id="688e4-134">String collection</span></span>|<span data-ttu-id="688e4-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="688e4-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="688e4-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="688e4-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="688e4-137">id</span><span class="sxs-lookup"><span data-stu-id="688e4-137">id</span></span>|<span data-ttu-id="688e4-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="688e4-138">String</span></span>|<span data-ttu-id="688e4-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="688e4-139">Key of the entity.</span></span> <span data-ttu-id="688e4-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="688e4-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="688e4-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="688e4-141">createdDateTime</span></span>|<span data-ttu-id="688e4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="688e4-142">DateTimeOffset</span></span>|<span data-ttu-id="688e4-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="688e4-143">DateTime the object was created.</span></span> <span data-ttu-id="688e4-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="688e4-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="688e4-145">description</span><span class="sxs-lookup"><span data-stu-id="688e4-145">description</span></span>|<span data-ttu-id="688e4-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="688e4-146">String</span></span>|<span data-ttu-id="688e4-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="688e4-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="688e4-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="688e4-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="688e4-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="688e4-149">lastModifiedDateTime</span></span>|<span data-ttu-id="688e4-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="688e4-150">DateTimeOffset</span></span>|<span data-ttu-id="688e4-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="688e4-151">DateTime the object was last modified.</span></span> <span data-ttu-id="688e4-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="688e4-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="688e4-153">displayName</span><span class="sxs-lookup"><span data-stu-id="688e4-153">displayName</span></span>|<span data-ttu-id="688e4-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="688e4-154">String</span></span>|<span data-ttu-id="688e4-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="688e4-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="688e4-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="688e4-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="688e4-157">version</span><span class="sxs-lookup"><span data-stu-id="688e4-157">version</span></span>|<span data-ttu-id="688e4-158">Int32</span><span class="sxs-lookup"><span data-stu-id="688e4-158">Int32</span></span>|<span data-ttu-id="688e4-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="688e4-159">Version of the device configuration.</span></span> <span data-ttu-id="688e4-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="688e4-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="688e4-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="688e4-161">Response</span></span>
<span data-ttu-id="688e4-162">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="688e4-162">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="688e4-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="688e4-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="688e4-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="688e4-164">Request</span></span>
<span data-ttu-id="688e4-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="688e4-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 225

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="688e4-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="688e4-166">Response</span></span>
<span data-ttu-id="688e4-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="688e4-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





