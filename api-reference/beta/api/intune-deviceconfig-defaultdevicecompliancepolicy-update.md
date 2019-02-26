---
title: Atualizar defaultDeviceCompliancePolicy
description: Atualiza as propriedades de um objeto defaultDeviceCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83b1c534c8b5e27e91bb6a1153f3b0a8f25496d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157698"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="f6cf8-103">Atualizar defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f6cf8-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="f6cf8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6cf8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6cf8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6cf8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6cf8-106">Atualiza as propriedades de um objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f6cf8-106">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6cf8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f6cf8-107">Prerequisites</span></span>
<span data-ttu-id="f6cf8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f6cf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f6cf8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6cf8-110">Permission type</span></span>|<span data-ttu-id="f6cf8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f6cf8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6cf8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6cf8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6cf8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6cf8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6cf8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6cf8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6cf8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6cf8-115">Not supported.</span></span>|
|<span data-ttu-id="f6cf8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6cf8-116">Application</span></span>|<span data-ttu-id="f6cf8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6cf8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6cf8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6cf8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="f6cf8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6cf8-119">Request headers</span></span>
|<span data-ttu-id="f6cf8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f6cf8-120">Header</span></span>|<span data-ttu-id="f6cf8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f6cf8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6cf8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6cf8-122">Authorization</span></span>|<span data-ttu-id="f6cf8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6cf8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6cf8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f6cf8-124">Accept</span></span>|<span data-ttu-id="f6cf8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f6cf8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6cf8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6cf8-126">Request body</span></span>
<span data-ttu-id="f6cf8-127">No corpo da solicitação, forneça uma representação JSON do objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f6cf8-127">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="f6cf8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f6cf8-128">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="f6cf8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6cf8-129">Property</span></span>|<span data-ttu-id="f6cf8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6cf8-130">Type</span></span>|<span data-ttu-id="f6cf8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6cf8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6cf8-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f6cf8-132">roleScopeTagIds</span></span>|<span data-ttu-id="f6cf8-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6cf8-133">String collection</span></span>|<span data-ttu-id="f6cf8-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f6cf8-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f6cf8-135">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6cf8-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6cf8-136">id</span><span class="sxs-lookup"><span data-stu-id="f6cf8-136">id</span></span>|<span data-ttu-id="f6cf8-137">String</span><span class="sxs-lookup"><span data-stu-id="f6cf8-137">String</span></span>|<span data-ttu-id="f6cf8-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f6cf8-138">Key of the entity.</span></span> <span data-ttu-id="f6cf8-139">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6cf8-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6cf8-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6cf8-140">createdDateTime</span></span>|<span data-ttu-id="f6cf8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6cf8-141">DateTimeOffset</span></span>|<span data-ttu-id="f6cf8-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f6cf8-142">DateTime the object was created.</span></span> <span data-ttu-id="f6cf8-143">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6cf8-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6cf8-144">description</span><span class="sxs-lookup"><span data-stu-id="f6cf8-144">description</span></span>|<span data-ttu-id="f6cf8-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6cf8-145">String</span></span>|<span data-ttu-id="f6cf8-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f6cf8-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f6cf8-147">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6cf8-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6cf8-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6cf8-148">lastModifiedDateTime</span></span>|<span data-ttu-id="f6cf8-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6cf8-149">DateTimeOffset</span></span>|<span data-ttu-id="f6cf8-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f6cf8-150">DateTime the object was last modified.</span></span> <span data-ttu-id="f6cf8-151">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6cf8-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6cf8-152">displayName</span><span class="sxs-lookup"><span data-stu-id="f6cf8-152">displayName</span></span>|<span data-ttu-id="f6cf8-153">String</span><span class="sxs-lookup"><span data-stu-id="f6cf8-153">String</span></span>|<span data-ttu-id="f6cf8-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f6cf8-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f6cf8-155">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6cf8-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6cf8-156">version</span><span class="sxs-lookup"><span data-stu-id="f6cf8-156">version</span></span>|<span data-ttu-id="f6cf8-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f6cf8-157">Int32</span></span>|<span data-ttu-id="f6cf8-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f6cf8-158">Version of the device configuration.</span></span> <span data-ttu-id="f6cf8-159">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6cf8-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f6cf8-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6cf8-160">Response</span></span>
<span data-ttu-id="f6cf8-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6cf8-161">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6cf8-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6cf8-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6cf8-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6cf8-163">Request</span></span>
<span data-ttu-id="f6cf8-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6cf8-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 229

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="f6cf8-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6cf8-165">Response</span></span>
<span data-ttu-id="f6cf8-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6cf8-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




